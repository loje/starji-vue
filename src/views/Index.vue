<template>
  <div class="home">
    <div class="index-top">
      <div class="index-nav">
        <div class="max-width">
          <div class="logo">
            <img src="@/assets/images/logo.svg" />
          </div>

          <div class="nav">
            <div class="menu-list">
              <div class="the-menu">下载</div>
              <div class="the-menu">浏览器插件</div>
              <div class="the-menu">用户案例</div>
              <div class="the-menu">使用教程</div>
              <div class="the-menu">帮助中心</div>
            </div>

            <div class="btn">注册账号</div>
          </div>
        </div>
      </div>
      <div class="top-main">
        <div class="t">灵感收集用星辑</div>
        <div class="desc">星辑随时随地的管理你的灵感库「图片、视频、音频素材等」，给你意向不到的快捷方便，同时也满足收藏、整理、查找，带来更高效的工作</div>
        <div class="btn-group">
          <div class="btn">
            <svg
              t="1598118314516"
              class="icon"
              viewBox="0 0 1024 1024"
              version="1.1"
              xmlns="http://www.w3.org/2000/svg"
              p-id="2233"
              width="16"
              height="16"
            >
              <path
                d="M666.871192 164.262228C703.626929 120.613835 727.208676 59.007858 721.981873 0c-52.497279 2.567553-118.107415 33.362899-154.863152 76.965443-34.096486 38.528571-62.981452 100.103981-55.11068 159.142406 57.769931 5.119822 118.107415-28.243078 154.909001-71.89147M939.841759 751.895524c-2.598119 5.119822-20.968345 74.428456-73.480907 146.258794-44.626508 61.62126-89.253016 125.74894-160.120521 125.74894-70.867506 0-91.8817-41.050274-173.218096-41.050274-81.351678 0-104.979275 41.050274-173.233378 41.050274-68.238821 2.552269-120.751383-69.293351-165.347325-130.868762C105.188517 764.763852 34.321011 533.791108 128.80083 377.216255c44.626508-76.934877 128.637437-128.255361 217.859886-128.255361 68.254104 0 131.235556 43.648393 173.218096 43.648393 42.028389 0 120.766666-56.501438 202.103061-46.215945 34.157618 2.567553 131.250839 12.807196 191.634171 102.656251-5.272652 2.567553-115.539863 66.725799-112.895894 195.027009 0 156.544287 136.508208 207.864771 139.121609 207.864771"
                fill="#ffffff"
                p-id="2234"
              />
            </svg>
            <span>免费下载MAC版</span>
          </div>
          <div class="btn">
            <svg
              t="1598118870514"
              class="icon"
              viewBox="0 0 1024 1024"
              version="1.1"
              xmlns="http://www.w3.org/2000/svg"
              p-id="3083"
              width="16"
              height="16"
            >
              <path
                d="M125.578 242.306v221.827l243.037-9.090v-263.231l-243.037 50.489zM470.948 163.537v286.463l428.852-15.821v-359.678l-428.852 89.037zM125.578 560.077v221.827l243.037 50.494v-263.232l-243.037-9.089zM470.948 574.211v286.463l428.852 89.037v-359.678l-428.852-15.821z"
                p-id="3084"
                fill="#ffffff"
              />
            </svg>
            <span>WIN即将诞生 …</span>
          </div>
        </div>

        <div v-swiper:mySwiper="swiperOption" class="swiper-banner">
          <div class="swiper-wrapper">
            <div class="swiper-slide" :key="$index" v-for="(banner, $index) in banners">
              <img :src="banner" />
            </div>
          </div>
          <div class="swiper-pagination"></div>

          <!-- 如果需要导航按钮 -->
          <div class="swiper-prev">
            <svg t="1598121318163" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3932" width="16" height="16"><path d="M243.506461 485.633534 243.506461 485.633534c-14.854001 14.540876-14.854001 38.152148 0 52.734978l483.281003 474.699737c14.852978 14.547016 38.917565 14.547016 53.708122 0 14.852978-14.539853 14.852978-38.181823 0-52.727815L324.063528 511.996419 780.494562 63.666729c14.852978-14.547016 14.852978-38.187963 0-52.734978-14.795674-14.575668-38.861284-14.575668-53.708122 0L243.506461 485.633534 243.506461 485.633534zM243.506461 485.633534" p-id="3933" fill="#ffffff"></path><path d="M243.506461 485.633534 243.506461 485.633534c-14.854001 14.540876-14.854001 38.152148 0 52.734978l483.281003 474.699737c14.852978 14.547016 38.917565 14.547016 53.708122 0 14.852978-14.539853 14.852978-38.181823 0-52.727815L324.063528 511.996419 780.494562 63.666729c14.852978-14.547016 14.852978-38.187963 0-52.734978-14.795674-14.575668-38.861284-14.575668-53.708122 0L243.506461 485.633534 243.506461 485.633534zM243.506461 485.633534" p-id="3934" fill="#ffffff"></path></svg>
          </div>
          <div class="swiper-next">
            <svg t="1598121610116" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="6658" width="16" height="16"><path d="M761.1648 503.0656c0 9.8304-3.7376 19.6608-11.2384 27.1616L349.696 930.4576a38.4 38.4 0 1 1-54.2976-54.2976l373.0688-373.0688L295.3984 129.9968a38.4 38.4 0 1 1 54.2976-54.2976L749.9264 475.904c7.5008 7.5264 11.2384 17.3568 11.2384 27.1616z" p-id="6659" fill="#ffffff"></path></svg>
          </div>
        </div>
      </div>
      <div class="index-bg"></div>
    </div>

    <div class="index-2 max-width">
      <div class="title-group">
        <div class="t">还在为平常收集灵感素材而烦恼吗？</div>
        <div class="t">一键收集，效率翻倍</div>
      </div>
      <div class="item-media">
        <div class="media-img">
          <img src="@/assets/images/top_img.jpg" />
        </div>
        <div class="media-right">
          <div class="media-title">解决寻找灵感中<br/>遇到的难题</div>
          <div class="media-desc">星辑能满足你在灵感管理上各种需求，数万张灵感图片、上百种分类，为您的灵感图贴上标签，寻找相似色的灵感，在这里体验到采集到的愉悦感</div>
        </div>
      </div>
      <div class="item-list">
        <div class="the-item">
          <img src="@/assets/images/undraw_collecting_fjjl.svg" />
          <div class="item-t">收藏网站图片，步骤太麻烦</div>
        </div>
        <div class="the-item">
          <img src="@/assets/images/undraw_content_team_3epn.svg" />
          <div class="item-t">电脑素材太多，整理很费时</div>
        </div>
        <div class="the-item">
          <img src="@/assets/images/undraw_quiz_nlyh.svg" />
          <div class="item-t">素材散落各处，时常找不到</div>
        </div>
      </div>
    </div>

    <div class="index-3 max-width">
      <div class="title">如何用星辑收集灵感？</div>
      <div class="desc">当你遇到值得收藏的灵感画面时，星集右击、拖拉的形式让你轻松保存，同时为他赋上标签，再也不用担心找不到而让你遗憾了</div>

      <div class="item-media">
        <div class="media-img">
          <img src="@/assets/images/top_img.jpg" />
        </div>
        <div class="media-right">
          <div class="func-list">
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_3_1.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">浏览器扩充</div>
                <div class="func-desc">通过使用浏览器上的扩充，轻松一键采集图</div>
              </div>
            </div>
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_3_2.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">屏幕截图</div>
                <div class="func-desc">用截屏的方式快速采集后保存，随时捕捉灵感</div>
              </div>
            </div>
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_3_3.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">拖图存放</div>
                <div class="func-desc">看到自己喜欢的图长按鼠标，拖至对话框便可采集</div>
              </div>
            </div>
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_3_4.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">复制粘贴</div>
                <div class="func-desc">常用的复制粘贴都能很轻松配合星集采好图</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="index-4 max-width">
      <div class="title">素材如何管理？</div>
      <div class="desc">面对大量的灵感时，也不免整理，星辑会通过标签、分类文件夹合理的将你采集的图为他们赋予属性，不在担心找不到很久之前采集到的灵感啦</div>

      <div class="item-media">
        <div class="media-img">
          <img src="@/assets/images/top_img.jpg" />
        </div>
        <div class="media-right">
          <div class="func-list">
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_4_1.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">分类文件夹</div>
                <div class="func-desc">通过个人的分类习惯将采集到的为分类分配到各个文件夹中</div>
              </div>
            </div>
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_4_2.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">图片标签</div>
                <div class="func-desc">为你心爱的灵感赋予他的属性，为你搜图更快一步</div>
              </div>
            </div>
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_4_3.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">筛选图库</div>
                <div class="func-desc">通过条件搜索匹配对应的灵感</div>
              </div>
            </div>
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_4_4.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">快捷搜素栏</div>
                <div class="func-desc">搜文件夹、标签，点哪搜哪</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="index-5 max-width">
      <div class="title">我们的体验？</div>
      <div class="desc">沉浸在星辰大海的图库里寻找你需要的灵感，行云流水，只需打开，灵感激发</div>

      <div class="item-media">
        <div class="media-img">
          <img src="@/assets/images/top_img.jpg" />
        </div>
        <div class="media-right">
          <div class="func-list">
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_5_1.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">单图、多图模式</div>
                <div class="func-desc">通过个人的分类习惯将采集到的为分类分配到各个文件夹中</div>
              </div>
            </div>
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_5_2.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">图片缩放</div>
                <div class="func-desc">通过对图片的缩放自如，更深入看到细节</div>
              </div>
            </div>
            <div class="the-func">
              <div class="func-img">
                <img src="@/assets/images/func_5_3.svg" />
              </div>
              <div class="func-right">
                <div class="func-t">瀑布流自适应的观赏</div>
                <div class="func-desc">让你对视觉的整齐感，沉浸在其中</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="index-gray">
      <div class="index-6 max-width">
        <div class="title">海量支持格式</div>
        <div class="desc">更多格式敬请期待</div>

        <div class="icon-list">
          <div class="the-icon">
            <img src="@/assets/images/JPG.svg" />
          </div>
          <div class="the-icon">
            <img src="@/assets/images/PNG.svg" />
          </div>
          <div class="the-icon">
            <img src="@/assets/images/SVG.svg" />
          </div>
          <div class="the-icon">
            <img src="@/assets/images/WEBP.svg" />
          </div>
          <div class="the-icon">
            <img src="@/assets/images/GIF.svg" />
          </div>
          <div class="the-icon">
            <img src="@/assets/images/EPS.svg" />
          </div>
        </div>
      </div>

      <div class="index-7 max-width">
        <div class="title">宅设工具粉丝榜推荐</div>
        <div class="desc">粉丝推荐</div>

        <div class="head-list">
          <div class="the-head"></div>
          <div class="the-head"></div>
          <div class="the-head"></div>
          <div class="the-head"></div>
          <div class="the-head"></div>
          <div class="the-head"></div>
          <div class="the-head"></div>
        </div>
      </div>

      <div class="index-8 max-width">
        <div class="the-content">
        <div class="title">立即开始免费使用</div>
        <div class="desc">一次性付费，采集终身使用，30天试用，功能不受限制</div>
        <div class="btn">立马试用</div>
        </div>
      </div>
    </div>

    <div class="bottom">
      <div class="max-width">
        <div class="btm-top">
          <div class="logo">
            <img src="@/assets/images/logo.svg" />
          </div>
          <div class="menu-list">
            <div class="the-menu">
              <div class="title">功能迭代</div>
              <div class="text">浏览器扩展</div>
              <div class="text">分类文件夹</div>
              <div class="text">兼容素材包</div>
              <div class="text">颜色筛选</div>
              <div class="text">标签管理</div>
            </div>
            <div class="the-menu">
              <div class="title">帮助中心</div>
              <div class="text">联系我们</div>
            </div>
            <div class="the-menu">
              <div class="title">商务合作</div>
              <div class="text">代理销售</div>
              <div class="text">活动赞助</div>
              <div class="text">培训机构</div>
              <div class="text">自媒体合作</div>
              <div class="text">社群合作</div>
            </div>
          </div>
        </div>
        <div class="btm-bottom">
          <span class="company">深圳市行星矩阵科技有限公司</span>
          <span class="icp">ICP备案号：xxxxxxxxxx</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import { directive } from "vue-awesome-swiper";
// If you use Swiper 6.0.0 or higher
import "@/assets/css/swiper-bundle.min.css";

export default {
  data() {
    return {
      banners: [require("@/assets/images/top_img.jpg"), require("@/assets/images/top_img.jpg")],
      swiperOption: {
        pagination: {
          el: ".swiper-pagination",
        },
        // 如果需要前进后退按钮
        navigation: {
          nextEl: '.swiper-next',
          prevEl: '.swiper-prev',
        },
      },
    };
  },
  mounted() {
    this.mySwiper.slideTo(3, 1000, false);
  },
  directives: {
    swiper: directive,
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
.max-width {
  margin: auto;
  width: 100%;
  max-width: 1000px;
}

.index-top {
  position: relative;
  .index-nav {
    position: relative;
    padding-top: 20px;
    width: 100%;
    z-index: 1;
    .max-width {
      display: flex;
      align-items: center;
      .logo {
        flex: 1;
        image {
          display: block;
          width: 118px;
          height: 48px;
        }
      }

      .nav {
        display: flex;
        .menu-list {
          display: flex;
          align-items: center;
          .the-menu {
            margin-right: 30px;
            color: #fff;
            font-size: 12px;
            cursor: pointer;
            &:hover {
              color: #fac220;
            }
          }
        }

        .btn {
          width: 86px;
          height: 30px;
          text-align: center;
          line-height: 28px;
          border: 1px solid #fff;
          color: #fff;
          font-size: 12px;
          border-radius: 4px;
          cursor: pointer;
          box-sizing: border-box;
          &:hover {
            color: #fac220;
            border-color: #fac220;
          }
        }
      }
    }
  }
  .top-main {
    position: relative;
    padding-top: 85px;
    text-align: center;
    z-index: 1;
    .t {
      font-size: 50px;
      line-height: 70px;
      color: #fca253;
    }
    .desc {
      margin: auto;
      margin-top: 8px;
      width: 502px;
      font-size: 14px;
      line-height: 28px;
      color: #fff;
    }

    .btn-group {
      display: flex;
      margin: auto;
      justify-content: space-between;
      margin: 36px auto;
      width: 398px;
      .btn {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 175px;
        height: 33px;
        line-height: 31px;
        border-radius: 33px;
        border: 1px solid #6d6d6d;
        color: #fff;
        text-align: center;
        font-size: 14px;
        cursor: pointer;
        box-sizing: border-box;
        .icon {
          margin-right: 11px;
        }
      }
    }

    .swiper-banner {
      margin: auto;
      width: 947px;
    }
  }
  .index-bg {
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 660px;
    background-color: rgb(61, 61, 61);
    z-index: 0;
  }
}

.swiper-prev {
  position: absolute;
  left: 12px;
  top: 238px;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 52px;
  height: 52px;
  border-radius: 50%;
  background-color: rgba(61, 61, 61, 0.36);
  z-index: 2;
  cursor: pointer;
  &:hover {
    background-color: rgba(252,162,83,0.36);
  }
}
.swiper-next {
  position: absolute;
  right: 12px;
  top: 238px;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 52px;
  height: 52px;
  border-radius: 50%;
  background-color: rgba(61, 61, 61, 0.36);
  z-index: 2;
  cursor: pointer;
  &:hover {
    background-color: rgba(252,162,83,0.36);
  }
}

.index-2 {
  padding-top: 60px;
  .title-group {
    margin-bottom: 34px;
    font-size: 30px;
    line-height: 42px;
    color: #333;
    text-align: center;
    font-weight: bold;
  }
  .item-media {
    display: flex;
    align-items: center;
    .media-img {
      width: 549px;
      height: 307px;
      img {
        width: 100%;
      }
    }
    .media-right {
      flex: 1;
      padding-left: 52px;
      .media-title {
        margin-bottom: 21px;
        font-size: 30px;
        line-height: 42px;
        color: #333;
      }
      .media-desc {
        color: #888;
        font-size: 14px;
        line-height: 25px;
      }
    }
  }
  .item-list {
    display: flex;
    align-items: baseline;
    padding-top: 70px;
    justify-content: space-between;
    .the-item {
      text-align: center;
      &:nth-child(1) {
        width: 219px;
      }
      &:nth-child(2) {
        width: 271px;
      }
      &:nth-child(3) {
        width: 279px;
      }
      img {
        display: block;
        width: 100%;
      }
      .item-t {
        margin-top: 21px;
        font-size: 14px;
        line-height: 20px;
        color: #333;
        text-align: center;
      }
    }
  }
}

.index-3 {
  padding-top: 70px;
  .desc {
    width: 469px;
  }
}
.index-4 {
  padding-top: 75px;
  .desc {
    width: 480px;
  }
}
.index-5 {
  padding: 75px 0;
  .desc {
    width: 352px;
  }
}
.index-3, .index-4, .index-5 {
  .title {
    margin-bottom: 7px;
    font-size: 30px;
    line-height: 42px;
    color: #333;
    text-align: center;
  }
  .desc {
    margin: auto;
    margin-bottom: 21px;
    font-size: 14px;
    line-height: 20px;
    color: #888;
    text-align: center;
  }
  .item-media {
    display: flex;
    align-items: center;
    .media-img {
      width: 549px;
      height: 307px;
      img {
        width: 100%;
      }
    }
    .media-right {
      flex: 1;
      padding-left: 20px;
      .func-list {
        .the-func {
          display: flex;
          align-items: center;
          margin-bottom: 5px;
          padding: 8px 15px;
          cursor: pointer;
          &:hover {
            background-color: rgba(232,232,232,0.37);
          }
          .func-img {
            width: 55px;
            height: 45px;
            img {
              display: block;
              width: 100%;
              height: 100%;
            }
          }
          .func-right {
            flex: 1;
            padding-left: 15px;
            box-sizing: border-box;
            .func-t {
              margin-bottom: 5px;
              font-size: 16px;
              line-height: 22px;
              color: #333;
            }
            .func-desc {
              font-size: 12px;
              line-height: 17px;
              color: #888;
            }
          }
        }
      }
    }
  }
}

.index-gray {
  padding: 75px 0;
  background-color: rgb(243, 243, 243);
  .index-6 {
    margin-bottom: 54px;
    .title {
      margin-bottom: 6px;
      font-size: 30px;
      line-height: 42px;
      color: #333;
      text-align: center;
    }
    .desc {
      margin-bottom: 21px;
      font-size: 12px;
      line-height: 17px;
      color: #888;
      text-align: center;
    }
    .icon-list {
      display: flex;
      justify-content: center;
      .the-icon {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 105px;
        height: 105px;
        border-radius: 10px;
        &:hover {
          background-color: #f8f8f8;
        }
        img {
          display: block;
          width: 56px;
        }
      }
    }
  }
  .index-7 {
    .title {
      margin-bottom: 6px;
      font-size: 30px;
      line-height: 42px;
      color: #333;
      text-align: center;
    }
    .desc {
      margin-bottom: 41px;
      font-size: 12px;
      line-height: 17px;
      color: #888;
      text-align: center;
    }

    .head-list {
      display: flex;
      height: 168px;
      margin-bottom: 87px;
      align-items: center;
      justify-content: space-between;
      .the-head {
        width: 106px;
        height: 106px;
        border-radius: 50%;
        background-color: #fff;
        transition: all ease 250ms;
        &:hover {
          width: 168px;
          height: 168px;
        }
      }
    }
  }

  .index-8 {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 780px;
    height: 297px;
    background-color: #fff;
    border-radius: 28px;
    .title {
      margin-bottom: 7px;
      font-size: 30px;
      line-height: 42px;
      color: #333;
    }
    .desc {
      margin-bottom: 41px;
      font-size: 14px;
      line-height: 20px;
      color: #333;
    }
    .btn {
      margin: auto;
      width: 174px;
      height: 45px;
      line-height: 45px;
      background-color: #fca253;
      border-radius: 23px;
      color: #fff;
      font-size: 24px;
      text-align: center;
    }
    .the-content {
      text-align: center;
    }
  }
}

.bottom{
  padding-top: 75px;
  padding-bottom: 40px;
  width: 100%;
  background-color: rgb(53, 53, 53);
  .max-width {
    .btm-top {
      display: flex;
      .logo {
        margin-right: 162px;
        img {
          display: block;
          width: 142px;
          height: 59px;
        }
      }
      .menu-list {
        display: flex;
        .the-menu {
          &:nth-child(1) {
            margin-right: 91px;
          }
          &:nth-child(2) {
            margin-right: 104px;
          }
          .title {
            margin-bottom: 18px;
            color: #CFCFCF;
            font-size: 20px;
            line-height: 28px;
          }
          .text {
            margin-bottom: 8px;
            color: #999;
            font-size: 14px;
            line-height: 20px;
            cursor: pointer;
          }
        }
      }
    }
    .btm-bottom {
      margin-top: 58px;
      color: #fff;
      font-size: 14px;
      line-height: 20px;
      .company {
        margin-right: 81px;
      }
    }
  }
}
</style>
