<!-- start here -->
<template>
    <div>
      <Header></Header>
      <StartHere></StartHere>
      <div class="start_here_main">
        <hgroup class="whitepaper_wrap">
          <div class="item-wrap whitepaper_info">
            <div class="whitepaper_title">WHITEPAPER</div>
            <div class="whitepaper_content">
              <a class="whitepaper-button show-lg whitepaper_download" data-title="DOWNLOAD" href="https://s3.ap-northeast-2.amazonaws.com/wp.s3.seele.pro/Seele_tech_whitepaper_EN_v2.0.pdf" target="_blank">
                <span><span >DOWNLOAD</span></span>
              </a>
            </div>
          </div>
        </hgroup>
        <hgroup class="features_wrap" id="SFeatures">
          <div class="box-title features_title">FEATURES</div>
          <div class="features_box_wrap">
            <div class="wrap features_box">
              <div class="features_img">
                  <img src="../assets/imgs/startHere/Algorithm.png" alt="">
              </div>
              <div class="features_info_wrap features_info_wrap_r">
                  <div class="features_info_title">NEURAL CONSENSUS ALGORITHM</div>
                  <div class="features_info_content">
                    <p>Seele created "Neural Consensus Algorithm". It transforms the consensus problem into an asynchronous request, 
                      processing and sorting data in a large-scale environment based on "micro-real numbers". </p>
                    <p>It will not only ensure 
                        safety and low energy consumption, but it will also ensure strong linear augmenting ability. The performance is linearly
                      accelerated as the node size increases to satisfy business requirements.
                    </p>
                  </div>             
              </div> 
            </div> 
          </div>
          <div class="features_box_wrap">
            <div class="wrap features_box">
               <div class="features_img features_img_sm_show">
                <img src="../assets/imgs/startHere/Network.png" alt="">
              </div>
              <div class="features_info_wrap features_info_wrap_l">
                <div class="features_info_title">HETEROGENEOUS FOREST NETWORK</div>
                <div class="features_info_content">
                  <p>Heterogeneous forest network is made up of different subnets.</p>
                  <p>Each subnet
                    can be seen as a stratified tree, which can handle the different service scenarios independently and interact with each other through cross-chain protocol.</p>
                </div>
              </div>
              <div class="features_img features_img_lg_show">
                <img src="../assets/imgs/startHere/Network.png" alt="">
              </div>
            </div>
          </div>
          <div class="features_box_wrap">
            <div class="wrap features_box">
              <div class="features_img">
                <img src="../assets/imgs/startHere/vtp.png" alt="">
              </div>
              <div class="features_info_wrap features_info_wrap_r">
                  <div class="features_info_title">Value Transport Protocol (VTP) and Value-Chain HTTP (VHTTP)</div>
                  <div class="features_info_content">
                    <p>VTP is based on the heterogeneous forest network architecture. The agreement covers the 
                      uniform identification of the assets on the chain and the routing strategy for asset discovery.</p>
                    <p>VHTTP implements the exchange of values among chains, between on-chain and off-chain.
                    </p>
                  </div>
              </div> 
            </div> 
          </div>
          <div class="features_box_wrap">
            <div class="wrap features_box">
              <div class="features_img features_img_sm_show">
                <img src="../assets/imgs/startHere/qvic.png" alt="">
              </div>
              <div class="features_info_wrap features_info_wrap_l">
                <div class="features_info_title">Quick Value Internet Connection (QVIC)</div>
                <div class="features_info_content">
                  <p>In the case of wide-area network, QVIC protocol conducts targeted optimization for network jitter, 
                    packet loss and other characteristics of instability. </p>
                  <p>QVIC protocol has greatly improved the transmission rate and efficiency, 
                    due to the use of pre-connection mode. 
                    As handshake control is done at the sending end, 
                    the handshaking time can be ignored. Data packets are transmitted directly, 
                    thus the greater efficiency is achieved.</p>
                </div>
              </div>
              <div class="features_img features_img_lg_show">
                <img src="../assets/imgs/startHere/qvic.png" alt="">
              </div>
            </div>
          </div>
        </hgroup>
      </div>
      <Footer></Footer>
    </div>
</template>
<script>
import Header from "./header";
import StartHere from "./itemBanner/startHere";
import Footer from "./footer";
export default {
  data() {
    return {};
  },
  components: {
    Header,
    StartHere,
    Footer
  }
};
</script>
<style lang="less">
.start_here_main {
  min-width: 1160px;
  .whitepaper_wrap {
    background: #eef3f5;
    display: flex;
    .whitepaper_info {
      position: relative;
    }
    .whitepaper_title {
      width: 40%;
      padding: 70px 0;
      color: #202020;
      font-size: 30px;
    }
    .whitepaper_content {
      .whitepaper_download {
        display: inline-block;
        position: absolute;
        top: 50%;
        right: 0;
        transform: translateY(-50%);
        letter-spacing: 1px;
        font-size: 18px;
        text-align: center;
        color: #fff;
      }
    }
  }
  .features_wrap {
    .features_box {
      display: flex;
      .features_img {
        width: 100%;
        height: 560px;
        img {
          width: 560px;
          height: 100%;
        }
      }
      .features_img_sm_show {
        display: none;
      }
      .features_img_lg_show {
        display: inline-block;
      }
      .features_info_title {
        width: 400px;
        font-size: 24px;
        color: #333;
        padding-bottom: 80px;
        font-weight: bold;
      }
      .features_info_content {
        line-height: 28px;
      }
      .features_info_content p:nth-child(2n + 1) {
        margin-bottom: 30px;
      }
      // .features_info_wrap:nth-child(2n) {
      //   padding-top: 130px;
      //   padding-left: 50px;
      // }
      // .features_info_wrap:nth-child(2n + 1) {
      //   padding-top: 130px;
      //   padding-right: 0px;
      //   text-align: left;
      //   .features_info_title {
      //     text-align: left;
      //   }
      // }
      .features_info_wrap_r{
        padding-top: 130px;
        padding-left: 50px;
      }
      .features_info_wrap_l{
        padding-top: 130px;
        padding-right: 50px;
      }
    }
    .features_box_wrap {
      padding: 60px 20px;
    }
    .features_box_wrap:nth-child(2n + 1) {
      background: #e7eaee;
    }
  }
}
@media screen and (min-width: 1024px) {
  .whitepaper-button {
    // display: inline-block;
    position: relative;
    width: 240px;
    height: 50px;
    font-size: 16px;
    /* border-radius: 30px; */
    margin-top: 0;
    z-index: 2;
    border: 2px solid #1346a2;
    cursor: pointer;
    color: #202020;
  }
  .whitepaper-button:hover {
    border: 2px solid #1346a2;
  }
  .whitepaper-button > span {
    display: block;
    position: absolute;
    overflow: hidden;
    left: 0;
    top: 0;
    width: 0%;
    height: 100%;
    /* border-radius: 30px; */
    -webkit-transition: 0.7s ease-in-out;
    -moz-transition: 0.7s ease-in-out;
    -o-transition: 0.7s ease-in-out;
    transition: 0.7s ease-in-out;
  }
  .whitepaper-button:after,
  .whitepaper-button > span > span {
    display: block;
    text-align: center;
    /* border-radius: 30px; */
    padding: 1em 0;
  }
  .whitepaper-button:after {
    content: attr(data-title);
    width: 100%;
    color: #202020;
  }
  .whitepaper-button > span > span {
    width: 244px;
    background: #1346a2;
    color: #fff;
  }
  .whitepaper-button:hover > span {
    /* border-radius: 30px; */
    margin-left: -2px;
    width: 102%;
  }
}
@media screen and (max-width: 768px) {
  .start_here_main {
    min-width: 100%;
    .whitepaper_wrap {
      width: 100%;
      display: inline-block;
      background: #eef3f5;
      .whitepaper_info {
        width: 100%;
        display: inline-block;
        position: relative;
      }
      .whitepaper_title {
        text-align: center;
        width: 100%;
        padding: 40px 0;
        color: #202020;
        font-size: 30px;
      }
      .whitepaper_content {
        text-align: center;
        margin-bottom: 40px;
        .whitepaper_download {
          text-align: center;
          display: inline-block;
          position: relative;
          top: 30px;
          width: 220px;
          height: 50px;
          line-height: 50px;
          background: #1346a2;
          letter-spacing: 1px;
          font-size: 18px;
          text-align: center;
          color: #fff;
        }
      }
    }
    .features_wrap {
      display: inline-block;
      .features_box {
        display: inline-block;
        text-align: center;
        .features_img {
          text-align: center;
          width: 100%;
          height: 320px;
          img {
            width: 320px;
            height: 320px;
          }
        }
        .features_img_sm_show {
          display: inline-block;
        }
        .features_img_lg_show {
          display: none;
        }
        .features_info_title {
          width: 100%;
          font-size: 22px;
          color: #333;
          padding: 30px 0px 20px 0px;
          font-weight: bold;
          text-align: left;
        }
        .features_info_content {
          font-size: 14px;
          color: #666;
          padding: 0px;
          text-align: left;
          line-height: 24px;
        }
        .features_info_content p:nth-child(2n + 1) {
          margin-bottom: 10px;
        }
        .features_info_wrap:nth-child(2n) {
          padding: 0;
        }
        .features_info_wrap:nth-child(2n + 1) {
          padding: 0;
          text-align: left;
          .features_info_title {
            text-align: left;
          }
        }
      }
      .features_box_wrap {
        padding: 40px 20px;
      }
      .features_box_wrap:nth-child(2n + 1) {
        background: #e7eaee;
      }
    }
  }
  .features_title {
    margin: 40px 0;
  }
}
</style>
      
