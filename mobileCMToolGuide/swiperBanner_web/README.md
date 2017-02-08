# Swiper Banner

좌우 스와이프 되는 배너 입니다





![그림참고](images/01.jpg)

html 파일


```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xmlns="http://www.w3.org/1999/html">
<head>
    <title>옥션 - 모바일 쇼핑은 옥션</title>
    <meta http-equiv="Content-Type" content="text/html; charset=euc-kr" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <link rel="stylesheet" href="http://eventimg.auction.co.kr/md/auction/08405BF42E/idangerous.swiper.css">
    <style type="text/css">
        *{margin:0;padding:0}
        img{border:0;vertical-align:top}
        li{list-style:none}

        #p_wrapper{width:980px;margin:0 auto;position:relative;padding-bottom:20px}     
        #p_wrapper .swiper-wrapper{position:relative}
        #p_wrapper .swiper-slide{position:relative;width:980px;height:500px;}
        #p_wrapper .swiper-pagination{width:100%;bottom:0;left:0}
        #p_wrapper .swiper-pagination .swiper-pagination-switch{width:12px;height:12px;display:inline-block;*display:inline;*zoom:1;padding:0 8px;background:url(http://eventimg.auction.co.kr/md/auction/08E93EF946/w_ico_blit_off.png) no-repeat 0 0;border-radius:0}
        #p_wrapper .swiper-pagination .swiper-active-switch{background:url(http://eventimg.auction.co.kr/md/auction/08E93EF946/w_ico_blit_on.png) no-repeat 0 0}
        #p_wrapper .swiper-button-prev{width:68px;height:68px;position:absolute;top:50%;margin-top:-34px;left:0;background:url(http://eventimg.auction.co.kr/md/auction/08E93EF946/w_btn_prev.png) no-repeat 0 0;z-index:100;cursor:pointer}
        #p_wrapper .swiper-button-next{width:68px;height:68px;position:absolute;top:50%;margin-top:-34px;right:0;background:url(http://eventimg.auction.co.kr/md/auction/08E93EF946/w_btn_next.png) no-repeat 0 0;z-index:100;cursor:pointer}
    </style>
    <script type="text/javascript" src="http://script.auction.co.kr/common/jquery.js"></script>
    <script src="http://eventimg.auction.co.kr/md/auction/08405BF42E/idangerous.swiper.js"></script>
</head>
<body>

   <div id="p_wrapper">

        <div class="swiper-container">
            <div class="swiper-wrapper">


                <div class="swiper-slide">
                    <img src="http://eventimg.auction.co.kr/md/auction/0944E1B900/ww3.jpg" usemap="#Map" border="0">
                    <map name="Map" id="Map">
                      <area shape="rect" coords="8,9,479,540" href="링크" target="_blank" />
                      <area shape="rect" coords="503,12,972,537" href="링크" target="_blank" />
                    </map>
                </div>

                <div class="swiper-slide">
                    <img src="http://eventimg.auction.co.kr/md/auction/0944E1B900/ww3.jpg" usemap="#Map2" border="0">
                    <map name="Map2" id="Map2">
                      <area shape="rect" coords="9,7,479,535" href="링크" target="_blank" />
                      <area shape="rect" coords="503,8,971,539" href="링크" target="_blank" />
                    </map>
                </div>

                <div class="swiper-slide">
                    <img src="http://eventimg.auction.co.kr/md/auction/0944E1B900/ww3.jpg" usemap="#Map3" border="0">
                    <map name="Map3" id="Map3">
                      <area shape="rect" coords="12,7,479,538" href="링크" target="_blank" />
                      <area shape="rect" coords="506,6,970,540" href="링크" target="_blank" />
                    </map>
                </div>
                


            </div>
        </div>

        <!-- Add Arrows -->
        <div class="swiper-button-prev"></div>
        <div class="swiper-button-next"></div>

        <!-- Add Pagination -->
        <div class="swiper-pagination"></div>

    </div>

    <script>
        var mySwiper = new Swiper('#p_wrapper .swiper-container', {         
            pagination:'#p_wrapper .swiper-pagination',
            paginationClickable:true,
            simulateTouch:true,
            loop:true,
            autoplay:4500,
            calculateHeight:true
        });
        $('#p_wrapper .swiper-button-prev').bind('click', function(e){
            e.preventDefault();

            // Autoplay false
            mySwiper.swipePrev();

            // Autoplay True
            mySwiper.stopAutoplay();
            mySwiper.swipePrev();
            mySwiper.startAutoplay();
        });
        $('#p_wrapper .swiper-button-next').bind('click', function(e){
            e.preventDefault();

            // Autoplay false
            mySwiper.swipeNext();

            // Autoplay True
            mySwiper.stopAutoplay();
            mySwiper.swipeNext();
            mySwiper.startAutoplay();
        });
    </script>

</body>
</html>
```


