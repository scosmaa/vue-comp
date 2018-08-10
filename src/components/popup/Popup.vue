<template>
    <div id="news_popup_timeline" class="mw-popup" ref="popupContainer">
        <span class="icon-mw-close btn-close-popup btn-close-popup-mobile" @click="close"></span>
        <div class="text">
            <div class="main-content">
                <div class="left-content">
                    <div class="image-container" ref="imageContainer" style="background-image: url('//newapp.marketwall.com/media/image/webNews/wn_66a28bc5-3e21-43e1-a054-3de8471c0edc.jpg')">
                        <iframe ref="sparkContent" class="hidden" style="width: 100%; height: 100%" frameborder="0"></iframe>
                        <iframe ref="videoContent" class="hidden" style="width: 100%; height: 100%" frameborder="0"></iframe>
                        <div class="hidden" ref="chartContent">
                            <div class="wn-back-header" style="padding: 10px;" ref="backHeader">
                                <div ref="infoContainer">
                                    <img ref="companyLogo" class="companyLogo wn-back-logo">
                                    <div class="wn-title-container" ref="backTitleContainer">
                                        <span class="main-wn-title" ref="title">&nbsp;</span>
                                        <span class="main-wn-var-perc" ref="variationTitle" style="display: none">&nbsp;</span>
                                    </div>

                                    <div class="wn-title-container wn-right back-subtitle-container" style="float: right" ref="backSubtitleContainer">
                                        <span class="main-wn-var-perc" ref="variation">&nbsp;</span>
                                        <span class="main-wn-value" ref="lastPrice">&nbsp;</span>
                                        <span class="main-currency" ref="currency">&nbsp;</span>
                                    </div>
                                </div>
                                <div style="margin-top: 3px">
                                    <span class="main-wn-public-code" ref="publicCode">&nbsp;</span>
                                    <span class="main-wn-last-update" ref="lastUpdate">&nbsp;</span>
                                </div>
                            </div>
                            <div class="hidden periods-container" ref="periodContainer">
                                <div class="period-table">
                                    <div class="row" ref="chartPeriodRow">
                                        <div class="period periodTD TD selected" ref="periodTD" data-period="TD">TODAY</div>
                                        <div class="period period1M" ref="period1M" data-period="1M">1M</div>
                                        <div class="period period3M" ref="period3M" data-period="3M">3M</div>
                                        <div class="period period6M" ref="period6M" data-period="6M">6M</div>
                                        <div class="period period1Y" ref="period1Y" data-period="1Y">1Y</div>
                                        <div class="period period3Y" ref="period3Y" data-period="3Y">3Y</div>
                                        <div class="period period5Y" ref="period5Y" data-period="5Y">5Y</div>
                                    </div>
                                </div>
                            </div>
                            <div ref="indexChart" data-dojo-type="app/widgets/MiddleLineAreaChart" data-dojo-props="showFrame:false,showLabel:false,showVariations:false"></div>
                            <div class="spinner-container" ref="chartLoadSpinner"></div>
                        </div>
                    </div>
                    <div class="main-title" ref="mainTitle">
                        UK – TASSO DI DISOCCUPAZIONE
                        <br> ILO SALE AL 4,4% A DICEMBRE
                    </div>
                    <div class="sub-title" ref="subTitle">
                        Feb 21 2018 13:44 | marketinsight.it
                    </div>
                    <div class="text-container-mobile" ref="textContainerMobile">
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
                            <span class=" noselect icon-mw-scale btn-scale" ></span>
                            <span class=" noselect btn-plus"> - </span>
                            <span class=" noselect btn-minus" > + </span>
                        </span>
                        <span>
                            <span class=" noselect icon-mw-invert btn-invert" ></span>
                            <span class=" noselect btn-invert-label"  ref="btnInvertLabel"></span>
                        </span>
                        <span ref="contentTypeButton" class="hidden">
                            <span class=" noselect btn-content fa"  ref="btnShowContentIcon"></span>
                            <span class=" noselect btn-invert-label uppercase"  ref="btnShowContentLabel"></span>
                        </span>
                        <span>
                        </span>
                    </div>
                </div>
                <div class="right-content">

                    <span class="icon-mw-close btn-close-popup" @click="close"></span>

                    <div style="position:relative; width: 100%; height:100%">

                        <div class="text-container" ref="textContainer" data-simplebar>
                            <div class="main-title main-title-spark" ref="mainTitleSpark">
                                UK – TASSO DI DISOCCUPAZIONE
                                <br> ILO SALE AL 4,4% A DICEMBRE
                            </div>
                            <div class="sub-title sub-title-spark" ref="subTitleSpark">
                                Feb 21 2018 13:44 | marketinsight.it
                            </div>
                            <div ref="textContainer">
                                AT&T has a rationale behind its recent acquisition spree.  The company wants to dominate the business of selling targeted advertising on internet-connected TVs and devices, according to advertising executives who have had conversations with the company. On the content side, AT&T acquired Time Warner for a whopping $85.4 billion, though the Department of Justice is suing to block the deal. It purchased entertainment company Otter Media for a price reported around $1 billion. It's also buying advertising tech such as the digital ad platform AppNexus, which it reportedly got for around $1.6 billion. AT&T has met with additional advertising technology companies about potential acquisitions.
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
   name: 'Popup',
   props: [ 'type' ],
   methods: {
       decreaseFontSize() {

       },
       increaseFontSize() {

       },
       close() {
            this.$refs.popupContainer.style.display = 'none';
            this.$destroy();
       },

   }
 }
</script>

<style lang="scss">
    @import 'style.scss'
</style>

