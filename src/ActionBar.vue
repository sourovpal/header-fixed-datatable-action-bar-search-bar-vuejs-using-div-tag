<script>

</script>

<template>

    <section class="action-bar">
        <div class="left-bar d-flex">
            <div class="item d-flex justify-content-center align-item-start wh-40">
                <label class="checkbox">
                    <input class="checkbox__input" type="checkbox">
                    <svg style="width:19px;height: 19px;" class="checkbox__icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 22 22"><rect width="21" height="21" x=".5" y=".5" fill="#FFF" stroke="#6499ff" rx="3" /><path class="tick" stroke="#1968ff" fill="none" stroke-linecap="round" stroke-width="4" d="M4 10l5 5 9-9" /></svg>
                </label>
            </div>
            <div class="item wh-40">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M17.65 6.35C16.2 4.9 14.21 4 12 4c-4.42 0-7.99 3.58-7.99 8s3.57 8 7.99 8c3.73 0 6.84-2.55 7.73-6h-2.08c-.82 2.33-3.04 4-5.65 4-3.31 0-6-2.69-6-6s2.69-6 6-6c1.66 0 3.14.69 4.22 1.78L13 11h7V4l-2.35 2.35z"></path> <path d="M0 0h24v24H0z" fill="none"></path></svg>
            </div>
        </div>
        <div class="right-bar d-flex">
            <div class="item wh-40">
                <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px"><path   d="M0 0h24v24H0z" fill="none"></path> <path   d="M10 18h4v-2h-4v2zM3 6v2h18V6H3zm3 7h12v-2H6v2z"></path></svg>
            </div>
            <div class="item d-none d-lg-flex">
                <button class="btn btn-primary shadow-none fw-bold">
                    <!-- <svg class="me-2" width="24" height="24" fill="#ffffff" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M19,13H13V19H11V13H5V11H11V5H13V11H19V13Z" /></svg> -->
                    <svg class="me-2" width="24" height="24" fill="#ffffff" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><title>account-plus</title><path d="M15,14C12.33,14 7,15.33 7,18V20H23V18C23,15.33 17.67,14 15,14M6,10V7H4V10H1V12H4V15H6V12H9V10M15,12A4,4 0 0,0 19,8A4,4 0 0,0 15,4A4,4 0 0,0 11,8A4,4 0 0,0 15,12Z" /></svg>
                    New Lead
                </button>
            </div>
            <div class="item d-none d-lg-flex">
                <div class="dropdown">
                    <button class="btn btn-light shadow-none fw-bold d-flex align-items-center" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        <span class="pe-4">Import</span>
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
            <div class="item d-none d-lg-flex wh-40">
                <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M3,5H8.3V19H3zM17,10c1.5,0,2.9,0.5,4,1.3V5h-5.3v5.1C16.1,10,16.5,10,17,10zM10,17c0-3,2-5.6,4.7-6.6V5H9.3v14h1C10.1,18.4,10,17.7,10,17zM20.8,17c0-0.2,0-0.4-0.1-0.6l1.1-1l-1-1.7l-1.5,0.5c-0.3-0.3-0.7-0.5-1.1-0.6L18,12h-2l-0.3,1.5c-0.4,0.1-0.8,0.4-1.1,0.6l-1.4-0.5l-1,1.7l1.1,1c0,0.2-0.1,0.4-0.1,0.6s0,0.4,0.1,0.6l-1.1,1l1,1.7l1.4-0.5c0.3,0.3,0.7,0.5,1.1,0.6L16,22h2l0.3-1.5c0.4-0.1,0.8-0.4,1.1-0.6l1.5,0.5l1-1.7l-1.1-1C20.7,17.4,20.8,17.2,20.8,17z M17,19c-1.1,0-2-0.9-2-2s0.9-2,2-2s2,0.9,2,2S18.1,19,17,19z"></path></svg>
            </div>
            <div class="wh-40 d-flex justify-content-center align-items-center fw-bold" style="min-width:4rem;">51-100</div>
            <div class="item wh-40">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M15.41 7.41L14 6l-6 6 6 6 1.41-1.41L10.83 12z"></path></svg>
            </div>
            <div class="item wh-40">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>

.action-bar{
    border-bottom: 1px solid rgba(182, 182, 182, 0.4);
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;

    .wh-40{
        width:40px;
        height:40px;
    }
    .right-bar,
    .left-bar{
        display: flex;
        justify-content:flex-start;
        align-items: center;
        .item{
            padding:10px 10px 10px 10px;
            display: flex;
            justify-content: flex-start;
            align-items: center;
            cursor: pointer;
            
            &.wh-40{
                position: relative;
                &::after{
                    content: "";
                    width: 38px;
                    height: 38px;
                    background-color: #e4eaef;
                    top: 50%;
                    left: 50%;
                    position: absolute;
                    transform: translate(-50%, -50%) scale(0);
                    border-radius: 50%;
                    z-index: -1;
                    transition: all 0.5s;
                }
                &:hover::after{
                    transform: translate(-50%, -50%) scale(1);
                }
            }
        }
    }
}
</style>
