<template>
    <div id="NewsInformation">
        <div class="container">
            <div class="container text-center">
                <h3>新闻动态</h3>
                <p style="color:#b2b2b2">Company News</p>
            </div>
            <div class="nav container text-center">
                <a href="#" class="active">公司新闻</a>
                <a href="#">行业动态</a>
            </div>
            <ul class="news-container container-fuild">
                <li v-for="(item,index) in newsList" :key="index" class="wow fadeIn">
                    <div class="content">
                        <p>{{item.title}}</p>
                        <p>{{item.introduce}}</p>
                    </div>
                    <div class="time">
                        <p>{{item.date}}</p>
                        <span>{{item.year}}</span>
                    </div>
                    <div class="circle">
                        <img src="../assets/img/circle.png">
                        <i class="line center-block"></i>
                    </div>
                </li>
            </ul>
            <div class="contaianer-fuild text-center more">
                <i class="glyphicon glyphicon-th"></i>
            </div>
        </div>
    </div>
</template>
<script>
import { WOW } from 'wowjs';
export default {
    name: 'NewsInformation',
    data() {
        return {
            newsList: [
                {
                    id: '001',
                    title: '公司创立',
                    introduce: '河南豫泽消防科技有限公司在行业中树立起标杆，致力于为客户提供卓越的消防科技解决方案。',
                    date: '08-08',
                    year: '2005'
                },
                {
                    id: '002',
                    title: '技术创新',
                    introduce: '公司在消防科技领域取得显著进展，引领行业发展潮流，推动技术的不断创新。',
                    date: '03-15',
                    year: '2007'
                },
                {
                    id: '003',
                    title: '市场拓展',
                    introduce: '公司逐步拓展市场，积极参与大型项目，为各类建筑和设施提供专业的消防安全解决方案。',
                    date: '07-20',
                    year: '2009'
                },
                {
                    id: '004',
                    title: '全球合作',
                    introduce: '公司加强国际合作，与世界各地的合作伙伴共同致力于全球消防科技事业的发展。',
                    date: '09-10',
                    year: '2013'
                },
                {
                    id: '005',
                    title: '荣誉殊荣',
                    introduce: '公司荣获多项行业荣誉，成为消防科技领域的杰出代表，受到业界高度认可。',
                    date: '12-05',
                    year: '2018'
                },
                {
                    id: '006',
                    title: '未来愿景',
                    introduce: '展望未来，公司将继续秉承创新精神，不断提升技术水平，为全球消防安全事业作出更大贡献。',
                    date: '02-28',
                    year: '2023'
                }
            ]

        }
    },
    mounted() {
        var wow = new WOW();
        wow.init();
    },
}
</script>
<style scoped>
.nav {
    margin: 20px 0;
}
.nav > a {
    display: inline-block;
    text-decoration: none;
    width: 120px;
    height: 45px;
    line-height: 45px;
    color: #333;
    border: 1px solid #333;
}
.nav > a.active {
    color: #1e73be;
    border-color: #1e73be;
}
.nav > a:hover {
    color: #1e73be;
    border-color: #1e73be;
}
.news-container {
    overflow: hidden;
    margin-bottom: 0;
}
.news-container > li {
    width: 55.6%;
    height: 120px;
    float: left;
    color: #333;
    text-align: right;
    border-left: 1px solid transparent;
    border-right: 1px solid transparent;
}
.news-container > li:hover {
    color: #1e73be;
    border: 1px solid #1e73be;
    cursor: pointer;
}
.news-container > li:nth-of-type(2n) {
    float: right;
    text-align: left;
}
.news-container > li > .content {
    width: 60%;
    float: left;
    padding: 20px 0;
}
.news-container > li > .time {
    width: 20%;
    float: left;
    padding: 10px 0;
}
.news-container > li > .time > p {
    font-size: 30px;
    margin: 5px 0;
}
.news-container > li > .circle {
    width: 20%;
    height: 100%;
    float: left;
    position: relative;
}
.news-container > li > .circle > img {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    margin: auto;
    width: 20px;
    height: 20px;
}
.news-container > li > .circle > i {
    display: block;
    width: 1px;
    height: 100%;
    background: #707070;
}
.news-container > li:nth-of-type(2n) > .content {
    float: right;
}
.news-container > li:nth-of-type(2n) > .time {
    float: right;
}
.news-container > li:nth-of-type(2n) > .circle {
    float: right;
}
.news-container > li:nth-of-type(1) > .circle > i {
    height: 50%;
    position: absolute;
    top: 50%;
    left: 50%;
}
.more {
    font-size: 25px;
    color: #707070;
}
.more > i {
    cursor: pointer;
}
@media screen and (max-width: 767px) {
    .news-container > li {
        width: 100%;
    }
    .news-container > li > .content {
        width: 70%;
        text-align: left;
        float: right;
    }
    .news-container > li > .time {
        width: 30%;
        text-align: left;
        float: right;
    }
    .news-container > li > .circle {
        display: none;
    }
}
</style>

