<template>
    <div class="@form_root">
        <div class="@form_container flex">
            <div class="@form_left_pane">
                <div class="@form_left_pad">
                    <div class="txt-fff">
                        <h3 class="@form_txt_caps s-28">Schedule a demo</h3>
                        <p>Learn more about FloQast.</p>
                    </div>
                </div>
            </div>
            <div class="@form_right_pane">
                <div class="@form_right_pad">
                    <div class="flex col center">
                        <div class="flex col">
                            <div class="@form_col_f">
                                <h3 class="@form_txt_grey txt-center">Learn How FloQast Can <span class="@form_emp">Improve Your Month-End</span></h3>
                            </div>
                            <div class="rel">
                                <div class="rel">
                                    <form class="mq flex" v-on:submit.prevent="onSubmit">
                                        <input type="text" placeholder="First Name*" class="@form_inp_name">
                                        <input type="text" placeholder="Email*" class="@form_inp_email">
                                        <input type="submit" value="SCHEDULE NOW" class="shared_bg txt-fff">
                                    </form>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style>
    @keyframes push_up {
        0%{
            transform: translateY(20px);
            opacity: 0
        }
        100%{
            transform: translateY(0);
            opacity: 1
        }
    }
    .rel{
        position: relative;
    }
    .\@form_root{
        width: 100%;
        position: absolute;
        left: 0;
        bottom: 50px;
        animation: push_up 622ms ease-in-out
    }
    .\@form_container{
        max-width: 943px;
        height: 106px;
        margin: 0 auto;
        background: #fbfbfb;
        border-radius: 5px;
        overflow: hidden;
        filter: drop-shadow(1.792px 4.668px 2.5px rgba(0,0,0,0.05))
    }
    .\@form_left_pane,
    .\@form_right_pane{
        text-transform: capitalize;
    }
    .\@form_left_pane{
        background: #8bc53f;
        line-height: 28px;
    }

    .\@form_left_pane {
        display: block;
        position: relative;
        float: left;
    }
    .\@form_left_pane:before {
        content: "";
        position: absolute;
        right: -20px;
        height: 0;
        width: 0;
        border-top: 53px solid transparent;
        border-bottom: 53px solid transparent;
        border-left: 21px solid #8bc53f;
        border-radius: 4px;
    }
    .\@form_left_pane p{
        font-size: 17px !important;
        font-weight: 400;
        font-style: normal;
    }
    h3{
        font-weight: 500;
    }
    .\@prim_theme_c{
        color: #8bc53f
    }
    .\@form_left_pad {
        padding: 24px 0px 26px 28px;
        margin-right: 20px
    }
    .\@form_right_pad{
        padding: 18px 24px 18px 38px
    }
    .\@form_col_f{
        margin-bottom: 15px;
    }
    .\@form_txt_caps{
        text-transform: uppercase;
    }
    .\@form_txt_grey{
        color: #6d6e70
    }
    .\@form_emp{
        color: #8bc53f
    }
    .shared_bg{
        background: #8bc53f
    }
    
    h3{
        font-size: 22px
    }
    .s-28{
        font-size: 24px
    }
    h3, p {
        margin: 0;
        white-space: nowrap;
    }

    input {
        border: 1px solid #dddddd;
        background: none;
        outline: none;
        font-size: 14px;
        padding: 5px 8px;
        border-radius: 3px;
        color: #3d3d3d !important
    }
    .\@form_inp_name,
    .\@form_inp_email{
        margin-right: 10px
    }
    input::placeholder{
        color: #b8b8b8
    }
    input[type=submit]{
        color: #fff !important;
        border: 2px solid #6f973b;
        border-radius: 4px !important;
        width: 213px
    }

    @media screen and (max-width: 943px){
        .\@form_root{
            left: 0;
            bottom: 0
        }
        .\@form_container{
            width: 100%;
            background: #fbfbfb;
            border-radius: 0;
            height: 100%
        }
        h3, p {
            white-space: normal;
        }
    }
    @media screen and (max-width: 942px){
        h3{
        font-size: 20px
        }
        .s-28{
            font-size: 22px
        }
    }
    @media screen and (max-width: 931px){
        .\@form_left_pane{
            display: none;
        }
        .\@form_right_pane{
            margin: 0 auto
        }
    }
    @media screen and (max-width: 710px){
        .mq{
            flex-direction: column;
        }
        input[type=submit]{
            width: 100%;
        }
        .\@form_inp_name,
        .\@form_inp_email{
            margin-right: 0;
            margin-bottom: 10px;
        }
    }
    @media screen and (max-width: 520px){
        .s-32{
            font-size: 27px
        }
        .s_48{
            font-size: 32px;
        }
    }
</style>