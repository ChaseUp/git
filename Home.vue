<style>
  @import "../css/reset";

  .userinfo-box {
    padding-top: 30px;
    height: 400px;
    background: #FFF url(../assets/userinfo_bg.png) no-repeat;
    background-size: 100% 100%;
    .avatar-box {
      display: block;
      width: 140px;
      height: 140px;
      border-radius: 50%;
      margin: 30px auto 0;
      position: relative;

      .avatar {
        display: block;
        width: 140px;
        height: 140px;
        margin: 0 auto;
        border-radius: 50%;
        border: 6px solid rgba(255,255,255,.3);
      }
    }
    .login {
      display: block;
      width: 6em;
      margin: 0 auto;
      padding: 20px 0 20px;
      text-align: center;
      font-size: 34px;
      color: #FFF;
    }
    .more {
      font-size: 28px;
      color: rgba(255,255,255,.8);
      text-align: center;
    }
    .open-txt {
      display: none;
    }
    .username {
      padding: 20px 0 20px;
      text-align: center;
      font-size: 34px;
      color: #FFF;

      .name {
        display: inline-block;
        height: 40px;
        line-height: 40px;
      }

      .vip-user-icon {
        display: inline-block;
        width: 50px;
        height: 40px;
        margin-left: 4px;
        vertical-align: bottom;
      }
    }
    .open {
      display: block;
      width: 240px;
      height: 52px;
      margin: 0 auto;
      border: 1px solid #FFF;
      border-radius: 30px;
      font-size: 28px;
      color: rgba(255,255,255,1);
      text-align: center;
      line-height: 52px;
    }
    .member-icon {
      display: -webkit-box;
      -webkit-box-align: center;
      -webkit-box-pack: center;
      margin-top: 6px;

      .icon {
        width: 54.6667px;
        height: 60px;
        margin: 0 5px;
        padding: 12.6667px 10px;
        background-image: url(../assets/medal_icon.png);
        background-size: 100% 400%;

        img {
          display: block;
          width: 100%;
          height: 100%;
        }
        &.vip img {
          display: none;
        }
        &.enjoy {
          background-position: 0 66.6666%;
        }
        &.support {
          background-position: 0 100%;
        }
      }
    }
  }
  .open-member {
    display: -webkit-box;
    -webkit-box-align: center;
    -webkit-box-pack: justify;
    height: 168px;
    margin-top: 16px;
    padding: 0 24px 0 30px;
    border-radius: 12px;
    font-size: 28px;
    color: rgba(255,255,255,.8);
    background-image: url(../assets/member_s_bg.png);
    background-size: 100% 300%;

    .icon {
      width: 82px;
      height: 90px;
      margin-right: 36px;
      padding: 18px 15px;
      background-image: url(../assets/medal_icon.png);
      background-size: 100% 400%;

      img {
        display: block;
        width: 100%;
        height: 100%;
      }
    }
    .info {
      -webkit-box-flex: 1;
      padding-right: 30px;

      p {
        height: 32px;
        line-height: 32px;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;

        &:first-child {
          margin-bottom: 20px;
          font-size: 32px;
          height: 36px;
          line-height: 36px;
          color: #fff;
        }
      }
    }
    .btn-open {
      display: block;
      width: 120px;
      height: 48px;
      border: 2px solid #FFF;
      border-radius: 30px;
      font-size: 28px;
      color: #fff;
      text-align: center;
      line-height: 48px;
    }
    &.vip .icon img {
      display: none;
    }
    &.enjoy {
      background-position: 0 50%;

      .icon {
        background-position: 0 66.6666%;
      }
    }
    &.support {
      background-position: 0 100%;

      .icon {
        background-position: 0 100%;
      }
    }
    &:first-of-type {
      margin-top: 0;
    }
  }
  .member-box {
    margin-top: 24px;
    padding: 30px 24px;
    background-color: #FFF;

    .title {
      position: relative;
      height: 106px;
      font-size: 30px;
      line-height: 106px;
      font-weight: bold;
      color: #202020;

      &::after {
        content: '';
        position: absolute;
        top: 50%;
        right: 0;
        left: 50%;
        border-top: 1px solid #E4E4E4;
      }
    }
  }
  .module-box {
    margin-top: 24px;
    background-color: #FFF;

    .module-title {
      display: block;
      position: relative;
      height: 112px;
      padding-left: 24px;
      border-bottom: 1px solid #E4E4E4;
      font-size: 34px;
      font-weight: bold;
      color: #333;
      line-height: 112px;

      .more-link {
        position: absolute;
        right: 20px;
        top: -webkit-calc(50% - 14px);
        padding-right: 23px;
        font-size: 28px;
        font-weight: normal;
        color: #999;
        background: url(../assets/arrow_grey.png) no-repeat right center;
        background-size: 16px 28px;
      }
      img {
        width: 46px;
        height: 46px;
        margin-right: 9px;
        vertical-align: middle;
      }
      &.no-border {
        border-bottom-style: none;
      }
      &.has-bg {
        background: url(../assets/arrow_grey.png) no-repeat -webkit-calc(100% - 24px) center;
        background-size: 16px 28px;
        font-weight: normal;
      }
    }
    .my-members {
      padding: 0 24px 16px;
    }
    .btn-other {
      display: block;
      width: 296px;
      height: 64px;
      margin: 16px auto 0;
      border: 1px solid #909090;
      border-radius: 45px;
      text-align: center;
      line-height: 64px;
      color: #333;
      font-size: 26px;
    }
    &.my-members-box {
      padding-bottom: 24px;
    }
  }
  .privilege-pad {
    display: none;
  }
  .privilege-box {
    display: -webkit-box;
    -webkit-box-align: center;
    height: 144px;

    .privilege-item {
      display: block;
      width: 33.333333%;
      padding-left: 27px;
      font-size: 28px;
      color: #666;

      .icon {
        display: inline-block;
        vertical-align: middle;
        width: 57px;
        height: 57px;
        margin-right: 12px;
        background: url(../assets/privilege.png) no-repeat;
        background-size: 100% 600%;

        &.privilege1 {
          background-position: 0 0;
        }
        &.privilege2 {
          background-position: 0 20%;
        }
        &.privilege3 {
          background-position: 0 40%;
        }
        &.privilege4 {
          background-position: 0 60%;
        }
        &.privilege5 {
          background-position: 0 80%;
        }
        &.privilege6 {
          background-position: 0 100%;
        }
      }
    }
  }
  .swiper-container {
    width: 100%;
    height: 170px;
  }
  .swiper-slide {
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: center;
    -webkit-box-pack: justify;
    padding: 30px 0 20px;
    border: 2px solid #E8EBF2;
    border-radius: 12px;
    background: url(../assets/star_blue.png) no-repeat right bottom;
    background-size: 100px 130px;

    img {
      display: block;
      width: 76px;
      height: auto;
    }
    p {
      max-width: 6em;
      padding-right: 20px;
      font-size: 28px;
      color: #666;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
      background: url(../assets/arrow_s.png) no-repeat right center;
      background-size: 11px 20px;
    }
  }
  @media screen and (min-width: 1000px) and (orientation: landscape) {
    .userinfo-box {
      display: -webkit-box;
      -webkit-box-align: center;
      -webkit-box-pack: justify;
      padding-top: 0;
      padding: 0 40px;
      border-bottom: 1px solid #E4E4E4;
      background: #fff;
      
      .avatar-box {
        margin: 0 30px 0 0;
      }
      .info {
        -webkit-box-flex: 1;
      }
      .username {
        color: #333;
        text-align: left;
        padding: 20px 0 20px;
      }
      .member-icon {
        -webkit-box-pack: start;
      }
      .login {
        margin: 0;
        color: #333;
        text-align: left;
      }
      .more {
        color: #666;
      }
      .open-txt {
        display: block;
        color: #666;
      }
      .open {
        margin: 0;
        background-color: #FF6740;
      }
    }
    .swiper-container {
      height: 150px;
    }
    .swiper-slide {
      padding: 20px 0 10px;
    }
    .privilege-phone {
      display: none;
    }
    .privilege-pad {
      display: block;
    }
    .privilege-box .privilege-item {
      width: 16.6667%;
      text-align: center;

      .icon {
        display: block;
        margin: 0 auto 20px;
      }
    }
  }
</style>

<template>
  <div class="home-page">
    <section class="userinfo-box">
      <a v-if="username" href="javascript:;" class="avatar-box">
        <img :src="avatar" onerror="this.src=''" class="avatar" @error="avatarErr" />
      </a>
      <a v-if="!username" href="javascript:;" class="avatar-box" @click="login">
        <img :src="avatar" onerror="this.src=''" class="avatar" @error="avatarErr" />
      </a>
      <template v-if="username">
        <div class="info">
          <p class="username">
            <span class="name">{{ nickname ? nickname : username }}</span>
            <img v-if="isVipUser" class="vip-user-icon" src="../assets/icon_membership_user.png" onerror="this.src=''">
          </p>
          <div class="member-icon" v-if="bought.length">
            <div class="icon" :class="getPackageType(item.packageType)" v-for="item in bought">
              <img :src="'http://img.mip.pplive.cn/' + item.logoUrl" onerror="this.src=''" />
            </div>
          </div>
          <p class="open-txt" v-else>立即开通会员，畅享精彩体育赛事</p>
        </div>
        <a href="openMain.html" id="sport_handle_sport_member" class="open" v-if="!bought.length">开通体育会员</a>
      </template>
      <div v-else>
        <a href="javascript:;" class="login" @click="login">登录 / 注册</a>
        <p class="more">登录可享受更多服务</p>
      </div>
    </section>
    <section class="member-box" v-if="bought.length == 0">
      <div class="open-member">
        <div class="icon"></div>
        <div class="info">
          <p>{{ vip.title }}</p>
          <p>{{ vip.description }}</p>
        </div>
        <a href="javascript:;" :id="buriedId" class="btn-open" @click="goOpenVipGuide">开通</a>
      </div>
      <p class="title">赛事畅享及球队死忠会员</p>
      <div class="swiper-container">
        <div class='swiper-wrapper'>
          <a href="javascript:;" class="swiper-slide" v-for="item in enjoyList" @click="goOpenBoth(item)">
            <img :src="item.logo" onerror="this.src=''" />
            <p>{{ item.title }}</p>
          </a>
        </div>
      </div>
    </section>
    <section class="module-box my-members-box" v-else>
      <p class="module-title no-border">
        我的会员<a href="mine.html" class="more-link" v-if="bought.length > 3">全部会员</a>
      </p>
      <div class="my-members" v-for="(item, index) in bought" v-if="index < 3">
        <div class="open-member" :class="getPackageType(item.packageType)">
          <div class="icon">
            <img :src="item.logoUrl" onerror="this.src=''" />
          </div>
          <div class="info">
            <p>{{ dealTitle(item) }}</p>
            <p>会员有效期至：{{ item.validDate.substring(0, 10) }}</p>
          </div>
          <a href="javascript:;" id="sport_renew" class="btn-open" @click="openContinue(item)">续费</a>
        </div>
      </div>
      <a class="btn-other" id="sport_handle_member_other" href="openMain.html">开通其他会员</a>
    </section>
    <section class="module-box">
      <p class="module-title">
        会员特权<a href="nsp.html" class="more-link">服务协议</a>
      </p>
      <div class="privilege-phone">
        <div class="privilege-box">
          <a href="privilege.html" class="privilege-item"><span class="icon privilege1"></span>专享比赛</a>
          <a href="privilege.html" class="privilege-item"><span class="icon privilege2"></span>可关闭广告</a>
          <a href="privilege.html" class="privilege-item"><span class="icon privilege3"></span>尊贵身份</a>
        </div>
        <div class="privilege-box">
          <a href="privilege.html" class="privilege-item"><span class="icon privilege4"></span>多端共享</a>
          <a href="privilege.html" class="privilege-item"><span class="icon privilege5"></span>赠送观赛券</a>
          <a href="privilege.html" class="privilege-item"><span class="icon privilege6"></span>专享活动</a>
        </div>
      </div>
      <div class="privilege-pad">
        <div class="privilege-box">
          <a href="privilege.html" class="privilege-item"><span class="icon privilege1"></span>专享比赛</a>
          <a href="privilege.html" class="privilege-item"><span class="icon privilege2"></span>可关闭广告</a>
          <a href="privilege.html" class="privilege-item"><span class="icon privilege3"></span>尊贵身份</a>
          <a href="privilege.html" class="privilege-item"><span class="icon privilege4"></span>多端共享</a>
          <a href="privilege.html" class="privilege-item"><span class="icon privilege5"></span>赠送观赛券</a>
          <a href="privilege.html" class="privilege-item"><span class="icon privilege6"></span>专享活动</a>
        </div>
      </div>
    </section>
    <section class="module-box" v-if="matchMore">
      <p class="module-title">
        专享比赛<a href="vipMatch.html" id="sport_more" class="more-link" v-if="matchMore">更多比赛</a>
      </p>
      <match date :list="matchList" />
    </section>
    <section class="module-box">
      <a class="module-title has-bg" id="sport_more_sport" href="qa.html"><img src="../assets/question.png" onerror="this.src=''"/>常见问题</a>
    </section>
    <loading ref="loading" />
    <loadingerr ref="loadingErr" />
  </div>
</template>

<script>
  import Match from 'components/Match'
  import Loading from 'components/Loading'
  import Loadingerr from 'components/LoadingErr'
  import common from 'js/common'
  import DI from 'js/interface'

  export default {
    components: {
      Match,
      Loading,
      Loadingerr,
    },
    data() {
      return {
        username: '',
        nickname: '',
        avatar: '',
        bought: [], // 已购买列表
        vip: {}, // vip会员信息
        enjoyList: [], // 赛事畅想及死忠列表
        matchList: [],
        matchMore: false,
        isVipUser: false
      }
    },
    computed: {
      buriedId() {
        return this.vip.title == '体育高级会员' ? 'sport_handle_senior_member' : (
               this.vip.title == '赛事畅享会员' ? 'sport_handle_match_member' : (
               this.vip.title == '球队死忠会员' ? 'sport_handle_team_member' : 'sport_handle_member'));
      }
    },
    methods: {
      avatarErr () {
        this.avatar = require('../assets/avatar.png');
      },
      login () {
        try{
          if(common.isPPTV){
            ppsdk.config({});
            ppsdk.ready(function() {
              ppsdk.login({
                autologin: false,
                success: function(data) {
                  const host = location.href.split('?')[0];
                  const agent = navigator.userAgent;
                  const appinfo = agent.substring(agent.indexOf('PPTV (') + 6).replace(/\)/g, '').split('; ');
                  location.href = host + '?username=' + data.userName + '&token=' + data.token + '&nickname=' + data.nickname + '&appver=' + data.nickname + '&appplt=' + data.nickname + '&appid=' + data.nickname;
                }
              })
            });
          }else{
            football.goLogin();
          }
        }catch(error) {
          console.log('请在app内打开')
        }
      },
      dealTitle (item) {
        let prefix = '';
        if(item.packageType == 0){
          prefix = '赛事畅享会员－';
        }else if(item.packageType == 1){
          prefix = '球队死忠－';
        }
        return prefix + item.packageName;
      },
      getPackages (type) {
        common.ajax({
          url: DI.packagList,
          data: {
            type: type,
            cataId: 38,
            format: 'jsonp',
          },
          dataType: 'jsonp',
          context: this,
          success: function(data) {
            if(data.root.list){
              if(type == 0){
                this.enjoyList = data.root.list;
                setTimeout(() => {
                  new Swiper('.swiper-container', {
                    slidesPerView: 3,
                    spaceBetween: 15
                  });
                }, 0);
              }else if(type == 2){
                this.vip = data.root.list[0]
              }
            }
          },
        });
      },
      getPackageType (type) {
        return common.getPackageType(type);
      },
      openContinue (item) {
        const locationSearch = '?packageid=' + item.packageId + '&renew=true';
        let locationHost = '';
        if(item.packageType == 0){ // 跳转开通专享页面
          locationHost = 'openEnjoy.html';
        }else if(item.packageType == 1){ // 跳转开通死忠页面
          locationHost = 'openSupport.html';
        }else if(item.packageType == 2){ // 跳转开通vip会员页面
          locationHost = 'openVip.html';
        }
        location.href = locationHost + locationSearch;
      },
      // goOpenMain () { // 跳转开通会员主页面
      //   location.href = 'openMain.html';
      // },
      goOpenVipGuide () { // 跳转开通vip会员页面
        if(this.username){
          location.href = 'openVip.html?packageid=' + this.vip.id;
        }else{
          this.login();
        }
      },
      goOpenBoth (item) { // 跳转开通专享和死忠页面
        if(this.username){
          if(item.isRelateTeam == 1){
            location.href = 'openEnjoyAndSupport.html?packageid=' + item.id;
          }else{
            location.href = 'openEnjoy.html?packageid=' + item.id;
          }
        }else{
          this.login();
        }
      },
      // goMine () { // 跳转我的全部会员页面
      //   location.href = 'mine.html';
      // },
      // goVipMatch () { // 跳转vip专享比赛页面
      //   location.href = 'vipMatch.html';
      // },
      // goPrivilege () { // 跳转vip专享比赛页面
      //   location.href = 'privilege.html';
      // },
    },
    mounted() {
      localStorage.removeItem('username');
      localStorage.removeItem('token');
      localStorage.removeItem('appver');
      localStorage.removeItem('appplt');
      localStorage.removeItem('appid');
      const params = common.getLocationSearch();

      this.username = params.username;
      this.nickname = params.nickname;
      this.avatar = decodeURIComponent(params.avatar);

      if(params.username){
        common.ajax({
          url: DI.bought,
          type: 'POST',
          data: {
            username: params.username,
            token: params.token,
            format: 'jsonp',
          },
          dataType: 'jsonp',
          jsonp: 'cb',
          context: this,
          success: function(data) {
            if(data.errorcode == 0){
              if(data.contents.length){
                this.bought = data.contents;
                this.isVipUser = true;
              }else{
                this.getPackages(0);
                this.getPackages(2);
              }
            }else{
              console.log(data.message);
            }
          },
        });
      }else{
        this.getPackages(0);
        this.getPackages(2);
      }
      common.ajax({
        url: DI.sectionList,
        type: 'POST',
        data: {
          payType: 0,
          app: 'h5',
          end: 3,
          start: 0,
        },
        dataType: 'jsonp',
        jsonp: '_callback',
        jsonpCallback: 'callback',
        context: this,
        success: function(data) {
          const list = Object.keys(data.data.list);
          if(list.length){
            const sections = data.data.list;
            let arr = [];
            for(let i=0; i<list.length; i++){
              if(arr.length == 3) break;
              const temp = sections[list[i]];
              if(temp.length){
                for(let j=0; j<temp.length; j++){
                  arr.push(temp[j]);
                  if(arr.length == 3) break;
                }
              }
            }
            if(arr.length == 3){
              this.matchMore = true;
              arr.pop();
            }
            this.matchList = arr;
          }
        },
      });
      common.buried();
    }
  }
</script>
