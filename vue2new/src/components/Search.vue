<template>
    <div class="card">
        <div class="card-header" align="center">
            <form class="form-inline">
                <input class="form-control form-control-lg wide" type="text" placeholder="搜索公众号/文章"><!--from-control 只要在form里面的控制器都是这样的-->
                <i class="fa fa-search btn btn-lg btn-outline-success" @click=""></i>
            </form>
        </div>
        <div class="card-block"> <!--总在新行上开始,高度,行高，顶和底边距都可控制,相反的inline就是在一行上高度不可I变-->
            <div class="media"> <!--媒体对象-->
                <div class="media-left imgbox">
                    <a class="" href="#">
                        <img class="media-object rounded"
                             src="http://dl.bizhi.sogou.com/images/2014/04/22/587880.jpg"> <!--媒体对象的图片,并且是左对齐-->
                    </a></div>
                <div class="media-body">

                    <h4>这个导演的新片，每一部我必二刷</h4>
                    <p class="text-muted" style="margin-bottom: 0px;">
                        11月的时候，鱼叔采访了自己的偶像——蒂姆·波顿。并有机会提前看到了他的新片，然后写了一篇推文。今天电影上映，鱼叔去电影院二刷。这一次，又
                    </p>
                    <p><small class="text-muted s1">
                        <span>    <i class="fa fa-star-o fa-lg float-xs-right text-danger"></i></span>
                        <i class="fa fa-eye"></i> 2348 </small>
                        <small class="text-muted">     独立鱼电影</small>
                        <small class="text-muted s2"> 1小时前</small>
                    </p>
                </div>
            </div>
            <div class="media">
                <div class="media-left imgbox">
                    <a class="" href="#">
                        <img class="media-object rounded "
                             src="http://wx.qlogo.cn/mmhead/Q3auHgzwzM6FDWDyWSNm2AFBwFV6SFMXa20hjbFlWOyGYFQqrryIPw/0">
                    </a></div>
                <div class="media-body">

                    <h4>现在的段子，不动脑子根本就看不懂</h4>
                    <p class="text-muted" style="margin-bottom: 0px;">
                        周末，姑妈让我帮忙表照顾5岁的表弟，晚上我给他洗澡的时候，女票打来电话。因为手不方便拿，就开了免提，她问:在做什么呢？我说...
                    </p>
                    <p><small class="text-muted s1">
                        <span>    <i class="fa fa-star-o fa-lg float-xs-right text-danger"></i></span>
                        <i class="fa fa-eye"></i> 1181 </small>
                        <small class="text-muted s1"> 凤凰网 </small>
                        <small class="text-muted s2"> 3小时前</small>
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
    .form-inline .wide {
        width: 80%;
    }
    .imgbox {
        width: 100px;
        height: 120px;
        overflow: hidden;
    }
    .imgbox img{
        max-width: 100px;
        /*max-height: 120px;*/
    }
    .s1 {
        margin-right: 20px;
    }
    .s2 {
        margin-left: 20px;
    }
</style>
