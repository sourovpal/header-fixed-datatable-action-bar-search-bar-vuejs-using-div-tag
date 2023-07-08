<script>

import ActionBar from './ActionBar.vue';
import SearchBar from './SearchBar.vue';

import vueCustomScrollbar from 'vue-custom-scrollbar/src/vue-scrollbar.vue'
import "vue-custom-scrollbar/dist/vueScrollbar.css";

export default {
  components: {
    vueCustomScrollbar,
    ActionBar,
    SearchBar
},
  data() {
    return {
      settings: {
        suppressScrollY: false,
        suppressScrollX: false,
        wheelPropagation: false
      }
    }
  },
  methods: {
    scrollHanle(evt) {
      // console.log(evt)
    }
  }
}
</script>

<template>
  <div class="container-fluid">
    <search-bar></search-bar>
    <action-bar></action-bar>
    <vue-custom-scrollbar class="tbl"  :settings="settings" @ps-scroll-y="scrollHanle">

        <div class="tbl-header d-none d-md-block">
            <div class="tbl-tr">
                <div class="tbl-th" style="width:3rem;"></div>
                <div class="tbl-th" style="width:5rem;">Avatar</div>
                <div class="tbl-th" style="width:20rem;">Lead</div>
                <div class="tbl-th">Source</div>
                <div class="tbl-th" style="width:5rem;">State</div>
                <div class="tbl-th" style="width:13.5rem;">Status</div>
                <div class="tbl-th">Name</div>
                <div class="tbl-th" style="width:9rem;">Phone Number</div>
                <div class="tbl-th" style="width:20rem;">Email Address</div>
                <div class="tbl-th" style="width:20rem;">Reocrd Link</div>
                <div class="tbl-th" style="width:20rem;">Note</div>
                <div class="tbl-th">Last Update</div>
                <div class="tbl-th">Created At</div>
            </div>
        </div>

        <section class="tbl-body">

            <div class="tbl-tr" v-for="item in Array.from(Array(100).keys())" :key="item">
                <div style="width:3rem;" class="tbl-td">
                  <label class="checkbox">
                    <input class="checkbox__input" type="checkbox">
                    <svg class="checkbox__icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 22 22"><rect width="21" height="21" x=".5" y=".5" fill="#FFF" stroke="#6499ff" rx="3" /><path class="tick" stroke="#1968ff" fill="none" stroke-linecap="round" stroke-width="4" d="M4 10l5 5 9-9" /></svg>
                  </label>
                </div>
                <div style="width:5rem;" class="tbl-td">
                  <img class="img-thumbnail" style="width:60px;" src="https://png.pngtree.com/png-vector/20220709/ourmid/pngtree-businessman-user-avatar-wearing-suit-with-red-tie-png-image_5809521.png">
                </div>
                <div style="width:20rem;" class="tbl-td">
                  <a class="text-decoration-none d-block w-100 py-1 text-overflow-ellipsis" href="">New {{ (item?item:1) * 2155 }} South Wales amet consectetur adipisicing elit.</a>
                </div>
                <div class="tbl-td">Powerman Local</div>
                <div class="tbl-td" style="width:5rem;"> {{ (item?item:1) * 2155 }}</div>
                <div class="tbl-td" style="width:13.5rem;">
                  <div class="dropdown w-100">
                    <button class="btn btn-light shadow-none fw-400 w-100 d-flex justify-content-between align-items-center" type="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        <span class="fw-bold text-fs tbl-dropdown-title">New</span>
                        <div class="dropdown--icon">
                          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M7 10l5 5 5-5z"></path> <path d="M0 0h24v24H0z" fill="none"></path></svg>
                        </div>
                    </button>
                    <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                  </div>
                </div>
                <div class="tbl-td">Powernam</div>
                <div style="width:9rem;" class="tbl-td">+88 {{item}}17123{{ (item?item:1) * 2155 }}</div>
                <div style="width:20rem;" class="tbl-td">
                  <span class="text-overflow-ellipsis">powermanlaocal@gmail.com</span>
                </div>
                <div style="width:20rem;" class="tbl-td">
                  <a class="text-decoration-none d-block w-100 py-1 text-overflow-ellipsis" href="https://png.pngtree.com/png-vector/20220709/ourmid/pngtree-businessman-user-avatar-wearing-suit-with-red-tie-png-image_5809521.png">https://png.pngtree.com/png-vector/20220709/ourmid/pngtree-businessman-user-avatar-wearing-suit-with-red-tie-png-image_5809521.png</a>
                </div>
                <div style="width:20rem;" class="tbl-td">
                  <span class="text-overflow-ellipsis">Lorem ipsum dolor sit amet consectetur adipisicing elit.</span>
                </div>
                <div class="tbl-td">05/07/2023</div>
                <div class="tbl-td">25/07/2023</div>
            </div>

        </section>

    </vue-custom-scrollbar>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css?family=Source+Sans+Pro:400,600');

*{
    font-family: 'Source Sans Pro', sans-serif;
}

html{
  scroll-behavior: smooth;
}
.ps__thumb-y{
  transition: all 0.1s;
}
.text-overflow-ellipsis{
  max-width: fit-content;
  overflow: hidden;
  text-overflow: ellipsis;
}
.btn-light{
  background-color:#edf1f5 !important;
}
.checkbox {
  cursor: pointer;
  display: flex;
  align-items: center;
}
.checkbox__input {
    position: absolute;
    width: 1.375em;
    height: 1.375em;
    opacity: 0;
    cursor: pointer;
}
.checkbox__input:checked + .checkbox__icon .tick {
  stroke-dashoffset: 0;
}
.checkbox__icon {
  width: 1.375em;
  height: 1.375em;
  flex-shrink: 0;
  overflow: visible;
}
.checkbox__icon .tick {
  stroke-dasharray: 20px;
  stroke-dashoffset: 20px;
  transition: stroke-dashoffset 0.2s ease-out;
}
.checkbox__label {
  margin-left: 0.5em;
}



.tbl{
  width:100%;
  overflow: hidden;
  overflow-x: auto;
  height: 600px;
}
.tbl-header{
  height:35px;
  position: sticky;
    top: 0;
    z-index: 9;
  }
  .tbl-header .tbl-tr{
    display: inline-flex;
    flex-direction: row;
  }
  .tbl-header .tbl-tr .tbl-th{
    border-bottom: 1px solid rgb(182 182 182 / 40%);
    display: flex;
    flex-direction: row;
    font-size: .875rem;
    font-weight: 700;
    color: #515253;
    width:10rem;
    padding: 6px 10px 6px 10px;
    cursor: pointer;
    white-space: nowrap;
    background-color: #ffffff;
  }
  .tbl-body{
    display: inline-block;
    padding-bottom:100px;
  }
.tbl-body .tbl-tr{
    display:inline-flex;
    flex-direction: row;
  }
  .tbl-body .tbl-tr .tbl-td{
    border-bottom: 1px solid rgb(182 182 182 / 40%);
    padding: 6px 10px 6px 10px;
    display: flex;
    flex-direction: row;
    font-size: 14px;
    font-weight: 400;
    width:10rem;
    white-space: nowrap;
    overflow: hidden;
    justify-content: flex-start;
    align-items: center;
    position: relative;
  }
  .tbl-body .tbl-tr .tbl-td,
  .tbl-body .tbl-tr .tbl-td a{
    color: #515253;
  }
  .tbl-body .tbl-tr:hover{
    background: rgb(182 182 182 / 12%);
  }
  .tbl .tbl-dropdown-title{
    font-size: 14px;
    max-width: 11rem;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    color: #515253;
  }
  .dropdown--icon svg{
    fill:#515253;
  }
</style>
