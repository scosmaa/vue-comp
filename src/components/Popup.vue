<template>
<div>
    <div id="news_popup_timeline" class="mw-popup" data-dojo-attach-point="popupContainer">
        <span class="icon-mw-close btn-close-popup btn-close-popup-mobile" data-dojo-attach-event="onClick:close"></span>
        <div class="text">
            <div class="main-content">
                <div class="left-content">
                    <div class="image-container" data-dojo-attach-point="imageContainer">
                        <iframe data-dojo-attach-point="sparkContent" class="hidden" style="width: 100%; height: 100%" frameborder="0"></iframe>
                        <iframe data-dojo-attach-point="videoContent" class="hidden" style="width: 100%; height: 100%" frameborder="0"></iframe>
                        <div class="hidden" data-dojo-attach-point="chartContent">
                            <div class="wn-back-header" style="padding: 10px;" data-dojo-attach-point="backHeader">
                                <div data-dojo-attach-point="infoContainer">
                                    <img data-dojo-attach-point="companyLogo" class="companyLogo wn-back-logo">
                                    <div class="wn-title-container" data-dojo-attach-point="backTitleContainer">
                                        <span class="main-wn-title" data-dojo-attach-point="title">&nbsp;</span>
                                        <span class="main-wn-var-perc" data-dojo-attach-point="variationTitle" style="display: none">&nbsp;</span>
                                    </div>

                                    <div class="wn-title-container wn-right back-subtitle-container" style="float: right" data-dojo-attach-point="backSubtitleContainer">
                                        <span class="main-wn-var-perc" data-dojo-attach-point="variation">&nbsp;</span>
                                        <span class="main-wn-value" data-dojo-attach-point="lastPrice">&nbsp;</span>
                                        <span class="main-currency" data-dojo-attach-point="currency">&nbsp;</span>
                                    </div>
                                </div>
                                <div style="margin-top: 3px">
                                    <span class="main-wn-public-code" data-dojo-attach-point="publicCode">&nbsp;</span>
                                    <span class="main-wn-last-update" data-dojo-attach-point="lastUpdate">&nbsp;</span>
                                </div>
                            </div>
                            <div class="hidden periods-container" data-dojo-attach-point="periodContainer">
                                <div class="period-table">
                                    <div class="row" data-dojo-attach-point="chartPeriodRow">
                                        <div class="period periodTD TD selected" data-dojo-attach-point="periodTD" data-period="TD">TODAY</div>
                                        <div class="period period1M" data-dojo-attach-point="period1M" data-period="1M">1M</div>
                                        <div class="period period3M" data-dojo-attach-point="period3M" data-period="3M">3M</div>
                                        <div class="period period6M" data-dojo-attach-point="period6M" data-period="6M">6M</div>
                                        <div class="period period1Y" data-dojo-attach-point="period1Y" data-period="1Y">1Y</div>
                                        <div class="period period3Y" data-dojo-attach-point="period3Y" data-period="3Y">3Y</div>
                                        <div class="period period5Y" data-dojo-attach-point="period5Y" data-period="5Y">5Y</div>
                                    </div>
                                </div>
                            </div>
                            <div data-dojo-attach-point="indexChart" data-dojo-type="app/widgets/MiddleLineAreaChart" data-dojo-props="showFrame:false,showLabel:false,showVariations:false"></div>
                            <div class="spinner-container" data-dojo-attach-point="chartLoadSpinner"></div>
                        </div>
                    </div>
                    <div class="main-title" data-dojo-attach-point="mainTitle">
                        UK – TASSO DI DISOCCUPAZIONE
                        <br> ILO SALE AL 4,4% A DICEMBRE
                    </div>
                    <div class="sub-title" data-dojo-attach-point="subTitle">
                        Feb 21 2018 13:44 | marketinsight.it
                    </div>
                    <div class="text-container-mobile" data-dojo-attach-point="textContainerMobile">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam sit amet ornare nisl, nec fermentum tellus. Curabitur ultrices
                        commodo ultrices. Donec auctor arcu id ligula porta, vel finibus purus efficitur. Aenean cursus elit
                        at nisi gravida porta. Pellentesque ante nunc, blandit eget magna quis, bibendum pretium nisl. Curabitur
                        ac enim vel arcu blandit facilisis. Fusce dignissim dignissim velit, vel egestas nulla molestie sed.
                        Quisque in aliquam nulla, at commodo massa. Proin euismod lectus eget porta vehicula.
                        <br>
                        <br> Morbi ornare, nisl faucibus pellentesque laoreet, enim lorem aliquet risus, ut malesuada justo tortor
                        id nisl. Suspendisse lectus libero, malesuada eu velit nec, mollis eleifend tortor. Aenean volutpat
                        posuere justo sed feugiat. Cras eu lacus nibh. Aenean fermentum ex et blandit malesuada. Sed blandit,
                        leo vitae facilisis pellentesque, risus velit vestibulum elit, eget posuere tellus quam commodo turpis.
                        Ut vulputate diam ut orci auctor consequat. Aenean efficitur, diam in fringilla accumsan, libero
                        purus egestas est, id congue mauris risus sit amet augue. Aenean tincidunt sit amet mauris sed dictum.
                        Nullam eu tempus purus. Curabitur ut condimentum purus. Fusce in mi pretium, ultrices justo sit amet,
                        sagittis velit. Sed condimentum facilisis pulvinar.
                        <br>
                        <br> Integer interdum vehicula nibh eu viverra. Ut gravida arcu quis quam viverra porta. Duis quis sapien
                        vitae nisi suscipit pharetra eget quis velit. Proin ultricies tincidunt tortor, eu hendrerit est
                        bibendum ut. In vitae finibus nulla, vitae lacinia odio. Nam facilisis arcu eget vulputate ultrices.
                        Nunc scelerisque, urna eget finibus sodales, eros est scelerisque sapien, eget scelerisque leo orci
                        eu est. Curabitur sed magna lectus.
                        <br>
                        <br> Praesent felis arcu, posuere et sem at, sollicitudin egestas eros. Etiam ut ex gravida, mollis sapien
                        at, pharetra arcu. Donec efficitur nec metus sit amet auctor. Vestibulum molestie, mauris porta pulvinar
                        ullamcorper, metus justo aliquet est, id luctus nulla dolor eu tellus. Curabitur aliquet convallis
                        urna, sed scelerisque tortor posuere luctus. Duis sollicitudin, risus quis eleifend molestie, nisi
                        lectus auctor mi, rhoncus sodales turpis purus nec urna. Donec in elit non enim pulvinar accumsan.
                        Praesent tellus ipsum, ullamcorper nec felis ac, maximus facilisis nisl. Suspendisse interdum diam
                        tempor lacinia tempor.
                        <br>
                        <br> Phasellus tempus neque velit, tristique finibus elit varius sed. Sed venenatis eu sem quis finibus.
                        Ut id nisi eget enim posuere porta. Aenean massa diam, egestas vitae tincidunt ac, pellentesque nec
                        sem. Ut eu nisl vel dui pretium condimentum tincidunt sed mauris. Pellentesque viverra lorem vitae
                        leo fermentum finibus. Vestibulum sit amet quam sollicitudin, aliquet mauris id, feugiat libero.
                        Maecenas accumsan nisl ultrices eros vulputate, ut vulputate eros sodales. Morbi vulputate gravida
                        dolor et facilisis. Sed sed quam sed nunc elementum varius nec vitae odio. Ut mattis rhoncus augue,
                        ut facilisis est facilisis sit amet. Etiam dapibus ullamcorper nulla. Aliquam eget ante tellus.
                        <br>
                        <br> Nunc blandit ligula massa. Aliquam ut lacinia sapien, ac mollis nibh. Praesent sollicitudin dictum
                        fermentum. Suspendisse faucibus suscipit justo non rhoncus. Nam blandit iaculis viverra. Aliquam
                        risus quam, vulputate id lorem non, tristique egestas libero. Aliquam sit amet tempor ex. Quisque
                        condimentum aliquet sem sit amet tincidunt. Pellentesque id tempor enim.
                        <br>
                        <br> Curabitur pellentesque ullamcorper enim malesuada aliquam. Nam vestibulum rutrum odio vitae facilisis.
                        Mauris nec nulla id lectus pulvinar cursus. Sed mi lacus, pulvinar vestibulum est volutpat, imperdiet
                        ornare ligula. Sed nec arcu tellus. Integer facilisis sapien ex, ut porta leo suscipit a. Nunc fringilla
                        porttitor semper. Donec semper metus urna, at dignissim ipsum finibus sit amet. Curabitur at est
                        et erat molestie sollicitudin ac eu lacus. Nunc ultricies pellentesque molestie. Sed sed pretium
                        nunc. Maecenas maximus lacus velit, et varius metus dictum a. Morbi lobortis ex posuere eros varius
                        mattis.
                        <br>
                        <br> Vestibulum quis enim porta dui feugiat consequat in sed mauris. Vestibulum ex tellus, porta elementum
                        dictum id, accumsan non lacus. Integer ac neque quis ante auctor sollicitudin. Proin mollis sodales
                        neque, vel pretium nisi rhoncus a. Pellentesque ac ipsum vel lectus suscipit posuere. Nullam vel
                        sem sed metus semper euismod nec et nisl. Donec pulvinar, ligula et lobortis vulputate, enim lectus
                        congue magna, ac ornare arcu nunc et dolor.
                        <br>
                        <br> Pellentesque cursus nisi ut est tristique pharetra. Curabitur pulvinar felis gravida porttitor tristique.
                        Cras et feugiat risus. Donec ullamcorper ut risus at pharetra. Nullam urna dolor, varius sit amet
                        accumsan eu, vehicula sed libero. Suspendisse pretium faucibus vestibulum. Sed tempus, magna at mattis
                        dignissim, leo mi suscipit ligula, a volutpat felis mauris vel lorem. Aliquam consectetur nunc non
                        lorem consequat, sed consectetur libero malesuada.
                        <br>
                        <br> Vestibulum tellus ex, ullamcorper vitae neque efficitur, tristique iaculis mauris. Nunc consequat
                        consequat felis in elementum. Suspendisse potenti. Donec dui purus, lacinia id fringilla non, dictum
                        et diam. In hac habitasse platea dictumst. Donec vestibulum magna nibh, ut egestas nunc porta non.
                        Duis ac rhoncus tellus, sed porta risus. Aenean quam purus, porttitor sit amet tortor vel, egestas
                        tristique est. Etiam ut erat ac sapien mattis fringilla vel et dolor. Nam vitae nisi ex. Maecenas
                        rhoncus sed neque nec eleifend.
                    </div>
                    <div class="action-bar">
                        <span>
                            <span class=" noselect icon-mw-scale btn-scale" data-dojo-attach-event="onClick:toggleFontSize"></span>
                            <span class=" noselect btn-plus" data-dojo-attach-event="onClick:decreaseFontSize"> - </span>
                            <span class=" noselect btn-minus" data-dojo-attach-event="onClick:increaseFontSize"> + </span>
                        </span>
                        <span>
                            <span class=" noselect icon-mw-invert btn-invert" data-dojo-attach-event="onClick:changeTone"></span>
                            <span class=" noselect btn-invert-label" data-dojo-attach-event="onClick:changeTone" data-dojo-attach-point="btnInvertLabel"></span>
                        </span>
                        <span data-dojo-attach-point="contentTypeButton" class="hidden">
                            <span class=" noselect btn-content fa" data-dojo-attach-event="onClick:showNextContent" data-dojo-attach-point="btnShowContentIcon"></span>
                            <span class=" noselect btn-invert-label uppercase" data-dojo-attach-event="onClick:showNextContent" data-dojo-attach-point="btnShowContentLabel"></span>
                        </span>
                        <span>
                        </span>
                    </div>
                </div>
                <div class="right-content">

                    <span class="icon-mw-close btn-close-popup" data-dojo-attach-event="onClick:close"></span>

                    <div style="position:relative; width: 100%; height:100%">

                        <div class="text-container" data-dojo-attach-point="textContainer" data-simplebar>
                            <div class="main-title main-title-spark" data-dojo-attach-point="mainTitleSpark">
                                UK – TASSO DI DISOCCUPAZIONE
                                <br> ILO SALE AL 4,4% A DICEMBRE
                            </div>
                            <div class="sub-title sub-title-spark" data-dojo-attach-point="subTitleSpark">
                                Feb 21 2018 13:44 | marketinsight.it
                            </div>
                            <div data-dojo-attach-point="textContainer"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    

}
</script>

<style lang="scss" scoped>
.mw-popup .periods-container,
.web-news-box .periods-container {
    width: 100%;
}
.mw-popup .periods-container .period-table .row,
.web-news-box .periods-container .period-table .row {
    display: table;
    width: 100%;
    padding: 10px;
    padding-top: 0;
    display: table;
    box-sizing: border-box;    
}

.mw-popup .periods-container .period-table .row .period,
.web-news-box .periods-container .period-table .row .period {
    display: table-cell;
    cursor: pointer;
    width: 14%;
    border: 1px solid #3c3c3c;
    text-align: center;
    padding-top: 6px;
    padding-bottom: 6px;
}

.mw-popup .periods-container .period-table .row .period.selected, 
.mw-popup .periods-container .period-table .row .period:hover,
.web-news-box .periods-container .period-table .row .period.selected, 
.web-news-box .periods-container .period-table .row .period:hover {
    background-color: #3c3c3c;
}
.spark-content .mw-popup .image-container {
    background-position-x: center;
    background-position-y: top;
    background-repeat: no-repeat;
    background-size: cover;
    height: 692px;
    margin-top: 60px;
    margin-left: 20px;
    margin-right: 20px;
    /* margin-bottom: 20px; */
    position: initial;
}

.spark-content .mw-popup .left-content {
    position: absolute;
    width: 50%;
    height: auto;
    top: 20px;
    bottom: 5px;
    box-sizing: border-box;
}
.mw-popup .main-content {
    width:100%;
    height: 100%;
    background-color: #282828;
    position: relative
}

.mw-popup .left-content {
    position: absolute;
    width: 50%;
    height: auto;
    left: 0px;
    top: 20px;
    bottom: 5px;
    box-sizing: border-box;
}

.mw-popup .right-content { 
    position: absolute;
    width: 50%;
    height: auto;
    right: 0px;
    top: 20px;
    bottom: 20px;
    padding-right: 25px;
    box-sizing: border-box;
}
.mw-popup .btn-close-popup {
    position: absolute; 
    right: 0; 
    top: 0; 
    z-index: 1; 
    font-size: 45px;
    margin-right: 20px;
    cursor: pointer;
} 
.mw-popup .image-container { 
    background-position-x: center;
    background-position-y: top;
    background-repeat: no-repeat;
    background-size: cover;
    height: 450px;
    margin-top: 50px;
    margin-left: 50px;
    margin-right: 20px;
    margin-bottom: 20px;
    position: initial;
}

.mw-popup .text-container-mobile,
.mw-popup .btn-close-popup-mobile {
    display: none
}

.mw-popup .text-container { 
    position: absolute;
    top: 50px;
    bottom: 0;
    /* overflow: auto; */
    line-height: 1.8;
    right: 20px;
    left: 20px;
    overflow-x: hidden;
}

.mw-popup .main-title {
    margin-left: 50px;
    margin-right: 20px;
    font-weight: bold;
    font-size: 35px;
    margin-top: 10px;
    color: rgb(69, 149, 247);
}
.mw-popup .main-title.main-title-spark {
    margin-top: 0;
}

.scroller {
    display: none
}

.spark-content  .scroller{
    position: absolute;
    margin: 0 auto;
    display: block;
    right: 50%;
    bottom: 0;
    margin-bottom: 80px;
}
.sub-title-spark,
.main-title-spark {
    display: none
}
.spark-content .mw-popup .main-title-spark,
.spark-content .mw-popup .sub-title-spark {
    margin-left: 0;
    display: block
}
.spark-content .mw-popup .sub-title {
    margin-bottom: 10px
}
.mw-popup .sub-title {
    margin-left: 50px;
    margin-top: 10px;
}

.mw-popup .action-bar {
    background-color: #333333;
    width:100%;
    bottom:0;
    height:50px;
    position: absolute;
}
.mw-popup .action-bar > span {
    width: 33.33%;
    float: left;
    height: 100%;
}

.mw-popup .action-bar .btn-scale {
    cursor: pointer;
    line-height: 50px;
    height: 100%;
    font-size: 26px;
    padding-left: 35px;
    margin-top: 4px;
    display: inline-block;
}

.mw-popup .action-bar .btn-invert {
    line-height: 50px;
    height: 100%;
    font-size: 18px;
    padding-left: 35px;
    margin-top: 4px;
    display: inline-block;
    cursor: pointer
}

.mw-popup .action-bar .btn-content {
    line-height: 50px;
    height: 100%;
    font-size: 18px;
    padding-left: 35px;
    margin-top: 4px;
    display: inline-block;
    cursor: pointer
}

.mw-popup .action-bar .btn-content-label {
    vertical-align: super;
    padding-left: 5px;
    display: inline-block;
    font-size: 15px;
    cursor: pointer
}

.mw-popup .action-bar .btn-invert-label {
    vertical-align: super;
    padding-left: 5px;
    display: inline-block;
    font-size: 15px;
    cursor: pointer
}

.mw-popup .action-bar .btn-plus, 
.mw-popup .action-bar .btn-minus {
    vertical-align: text-bottom;
    padding-left: 5px;
    text-align: center;
    display: inline-block;
    padding-top: 3px;
    font-size: 26px;
    cursor: pointer;
    color: rgb(69, 149, 247);
}

.mw-popup .action-bar .btn-plus {
    vertical-align: super;
}

.mw-popup.clear-tone .main-content,
.mw-popup.clear-tone .action-bar,
.mw-popup.clear-tone .action-bar .btn-plus, 
.mw-popup.clear-tone .action-bar .btn-minus {
    background-color: #fff;
    color: #000;
}
.mw-popup.clear-tone .image-container {
    -webkit-filter: grayscale(100%); /* Safari 6.0 - 9.0 */
    filter: grayscale(100%);
}
.mw-popup.clear-tone .text-container,
.mw-popup.clear-tone .main-title,
.mw-popup.clear-tone .sub-title,
.mw-popup.clear-tone .btn-close-popup {
    color: #000;
}

@media (max-width: 1400px) {
    .mw-popup .image-container {
        margin-top: 40px;
        height: 280px
    }

    .mw-popup .text-container {
        top: 25px;
    }

    .mw-popup .btn-close-popup {
        font-size: 30px;
        margin-right: 10px;
    }

    .mw-popup .main-title {
        font-size: 20px;
    }

    .spark-content .mw-popup .image-container {
        margin-top: 40px;
        height: 400px;
    }
}

@media (max-width: 1200px) {
    #news_popup_timeline .text {
        top: 25px !important;
        bottom: 25px !important;
        left: 20px !important;
        right: 20px !important;
    }

    .mw-popup .btn-close-popup {
        margin-right: 5px;
        margin-top: -15px;
    }

    .mw-popup .text-container {
        right: 0
    }

    .mw-popup .image-container,
    .mw-popup .main-title,
    .mw-popup .sub-title {
        margin-left: 25px;
    }
}

@media (max-width: 950px) {
    .mw-popup .action-bar {
        height: 30px;
    }
    .mw-popup .action-bar .btn-scale {
        line-height: 30px;
        font-size: 20px;
        padding-left: 25px;
        display: inline-block;
    }
    .mw-popup .action-bar .btn-plus, 
    .mw-popup .action-bar .btn-minus {
        font-size: 17px;
    }
    .mw-popup .action-bar .btn-plus {
        vertical-align: super
    }
    .mw-popup .action-bar .btn-invert {
        line-height: 30px;
        font-size: 13px;
        padding-left: 20px;
    }
    .mw-popup .action-bar .btn-invert-label {
        vertical-align: text-top;
        font-size: 11px;
    }
}

@media (max-width: 750px) {
    #news_popup_timeline .text {
        top: 0 !important;
        bottom: 0 !important;
        left: 0 !important;
        right: 0 !important;
    }


}

@media (max-width: 500px) {
    .sub-title-spark,
    .main-title-spark {
        display: none
    }
    .spark-content .mw-popup .image-container {
        margin-top: 40px;
        height: 280px;
        margin-left: 0;

    }
    .spark-content .left-content .main-title, .spark-content .left-content .sub-title {
        display: block;
    }

    .spark-content .mw-popup .left-content, .spark-content .mw-popup .right-content {
        width: 100%;
    }
    #news_popup_timeline .text {
        top: 0 !important;
        bottom: 0 !important;
        left: 0 !important;
        right: 0 !important;
    }
    .mw-popup .action-bar .btn-plus,
    .mw-popup .action-bar .btn-minus,
    .mw-popup .action-bar .btn-invert-label {
        display: none;
    }

    .mw-popup .action-bar {
        position: fixed;
        width: 100%;
        height: 50px;
        top: 0;

        -webkit-box-shadow: 0px 1px 5px 0px rgba(50, 50, 50, 0.4);
        -moz-box-shadow:    0px 1px 5px 0px rgba(50, 50, 50, 0.4);
        box-shadow:         0px 1px 5px 0px rgba(50, 50, 50, 0.4);
    }
    .mw-popup .left-content,
    .mw-popup .right-content {
        width: 100%;
    }
    .mw-popup .text-container {
        display: none
    }

    .mw-popup .btn-close-popup {
        font-size: 25px;
        margin-right: 10px;
        margin-top: -10px;
    }

    .mw-popup .action-bar .btn-scale {
        line-height: 49px;
        font-size: 34px;
        padding-left: 11px;
    }

    .mw-popup .text-container-mobile {
        display: block;
        margin: 70px 25px 0px;
    }

    .mw-popup .btn-close-popup-mobile {
        display: block;
        position: fixed;
        top: 23px;
        font-size: 24px;
        right: 0
    }
    .mw-popup .main-content {
        overflow: auto;
    }
    .mw-popup .image-container {
        width: 100%;
        margin: 0;
        margin-top: 30px;
        height: 230px;
    }
    .mw-popup .action-bar .btn-invert {
        width: 100%;
        padding-left: 0;
        text-align: center;
        line-height: 48px;
        font-size: 23px;
    }

    .mw-popup .right-content {
        display: none;
    }

    .multi-content-popup .mw-popup .action-bar > span {
        width: 25%;
    }
}
</style>

