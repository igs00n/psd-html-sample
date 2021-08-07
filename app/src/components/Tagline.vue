<template>
    <div class="@tagline_root">
        <div class="@tagline_container">
            <div class="@tagline_pad">
                <svg version="1.1" baseProfile="tiny-ps" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 256 65" width="256" height="65">
                    <defs>
                        <image  width="256" height="65" id="img1" href="data:image/png;base64,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"/>
                    </defs>
                    <g>
                        <g>
                            <g>
                                <use href="#img1" x="0" y="0" />
                            </g>
                        </g>
                    </g>
                </svg>
                <span class="s_32 @c-3f f-italic @the">The</span><br>
                <span class="@prim_theme_c s_48 f-mitalic">Fastest, Most Accurate</span><br>
                <span class="s_32 @c-3f f-italic">Way to Close Your Books!</span>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style scoped>
    @keyframes push_right {
        0%{
            transform: translateX(-20px);
            opacity: 0
        }
        100%{
            transform: translateX(0);
            opacity: 1
        }
    }
    .\@tagline_root{
        position: absolute;
        width: 60%;
        top: 120px;
        left: 0;
        animation: push_right 622ms ease-in-out
    }
    .\@tagline_container{
        background-image: linear-gradient(to right, rgba(255,255,255,.8) 50%, transparent)
    }
    .\@tagline_pad{
        padding: 30px 0;
        margin-left: 250px
    }
    .\@the{
        margin-left: 11px
    }
    .\@c-3f{
        color: #3f3f3f
    }
    .s_48{
        font-size: 42px
    }
    .s_32{
        font-size: 28px;
    }

    .f-italic{
        font-family: 'Roboto';
        font-weight: 500;
        font-style: italic
    }
    .f-mitalic{
        font-family: 'Roboto';
        font-weight: 500;
        font-style: italic
    }
    @media screen and (min-width: 1418px){
        .\@tagline_pad{
            padding: 30px 0;
            margin-left: 320px
        }
    }
    @media screen and (max-width: 1417px){
        .\@tagline_pad{
            padding: 30px 0;
            margin-left: 180px
        }
    }
    @media screen and (max-width: 1162px){
        .\@tagline_pad{
            padding: 30px 0;
            margin-left: 140px
        }
    }
    @media screen and (min-width: 1024px ) and (min-height: 1366px){
        .\@tagline_root{
            top: 320px;
        }
    }
    @media screen and (max-width: 1057px){
        .\@tagline_pad{
            padding: 30px 0;
            margin-left: 110px
        }
    }
    @media screen and (max-width: 943px){
        .\@tagline_root{
            width: 100%;
            height: 100%;
            top: 0;
            left:0
        }
        .\@tagline_container{
            width: 100%;
            height: 100%;
            background-image: none;
            background: rgba(255,255,255,.8) !important;
        }
        .\@tagline_pad{
            padding: 150px 0 0 0;
            margin-left: 0;
            text-align: center;
        }
    }
    @media screen and (max-width: 520px){
        .s_32{
            font-size: 27px
        }
        .s_48{
            font-size: 32px;
        }
    }
    @media screen and (max-width: 410px){
        .s_32{
            font-size: 22px
        }
        .s_48{
            font-size: 27px;
        }
        svg{
            width: 128px;
            height: 32.5px
        }
    }
</style>