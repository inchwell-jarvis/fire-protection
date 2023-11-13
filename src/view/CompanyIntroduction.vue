<template>
    <div id="CompanyIntroduction">
        <div class="banner container-fuild text-center">关于我们</div>
        <div class="container">
            <div class="row CompanyIntroduction-container">
                <div class="col-xs-12 col-sm-12 col-md-6 wow zoomIn">
                    <img class="img-responsive center-block" src="@/assets/img/about_img.png">
                </div>
                <div class="col-xs-12 col-sm-12 col-md-6">
                    <h3>河南豫泽消防科技有限公司</h3>
                    <p class=".text-justify">河南豫泽消防科技有限公司是一家专业致力于提供全方位消防安全解决方案的企业。我们拥有一支高效专业的团队，凭借先进技术和卓越服务，为客户提供各类消防产品和服务。我们的核心业务包括消防设备供应，系统设计与安装，维护服务以及培训等一站式解决方案。通过我们的努力，客户可以获得最优质的消防设备、个性化系统设计和安装、可靠的维护服务，以及专业的培训，确保在任何紧急情况下都能够迅速、有效地采取应对措施。</p>
                    <p class=".text-justify">我们的使命是通过创新和卓越的服务，为社会创造更安全的生活环境。我们致力于确保每个人都能在安全的条件下工作和生活。无论是提供高质量的消防设备，还是通过专业的培训提升社会对火灾防范的认知，河南豫泽消防科技有限公司始终秉持着为客户创造最佳消防解决方案的承诺。通过我们的努力，我们希望能够为社会的安全贡献一份力量，使每个角落都充满安全与信心。</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import { WOW } from 'wowjs';
export default {
    name: 'CompanyIntroduction',
    data(){
        return{

        }
    },
    mounted(){
        var wow = new WOW();
        wow.init();
    }
}
</script>
<style scoped>
.banner{
    color: #fff;
    font-size: 30px;
    height: 150px;
    line-height: 150px;
    background-image: url('../assets/img/banner1.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: scroll;
    background-position: center center;
}
.row{
    margin-right: 0;
    margin-left: 0;
}
.CompanyIntroduction-container{
    padding: 100px 0;
    color: #808080;
    transition: all ease 0.5s;
}
.CompanyIntroduction-container>div>p{
    font-size: 14px;
    line-height: 2.5rem;
}
@media screen and (max-width: 997px){
    .CompanyIntroduction-container{
    padding: 10px 0;
    color: #808080;
}
}
</style>

