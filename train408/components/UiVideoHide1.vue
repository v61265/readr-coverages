<template>
  <div class="video">
    <div id="0bc5857a-5469-4ea1-9ea5-3e565eeffdfd"></div>
  </div>
</template>

<script>
export default {
  head() {
    return {
      script: [
        {
          hid: 'hide1',
          async: true,
          innerHTML: `   
            (function() {
              var namespace = '__twreporterEmbeddedData';
              var pkg = 'scrollable-video';
              if (typeof window != 'undefined') {
                if (!window.hasOwnProperty(namespace)) {
                  window[namespace] = {};
                }
                if (window[namespace] && !window[namespace].hasOwnProperty(pkg)) {
                  window[namespace][pkg] = [];
                }
                if (Array.isArray(window[namespace][pkg])) {
                  var data = {"video":{"sources":[{"type":"video\u002Fmp4","src":"https:\u002F\u002Fstorage.googleapis.com\u002Fdata-journalism-public\u002F2021_train\u002Ftrain_hide1_1280.mp4","width":1280,"height":720},{"type":"video\u002Fmp4","src":"https:\u002F\u002Fstorage.googleapis.com\u002Fdata-journalism-public\u002F2021_train\u002Ftrain_hide1_1440.mp4","width":1440,"height":810},{"type":"video\u002Fmp4","src":"https:\u002F\u002Fstorage.googleapis.com\u002Fdata-journalism-public\u002F2021_train\u002Ftrain_hide1_1920.mp4","width":1920,"height":1080},{"type":"video\u002Fmp4","src":"https:\u002F\u002Fstorage.googleapis.com\u002Fdata-journalism-public\u002F2021_train\u002Ftrain_hide1_720.mp4","width":720,"height":1080},{"type":"video\u002Fmp4","src":"https:\u002F\u002Fstorage.googleapis.com\u002Fdata-journalism-public\u002F2021_train\u002Ftrain_hide1_960.mp4","width":960,"height":1440}]},"captions":[{"text":"這個造成多人喪命的工程，來自行政院 2014 年核定的「鐵路行車安全改善六年計畫」，原是希望改善邊坡的安全性，卻因施工不當釀成悲劇⋯⋯","time":0,"textAlign":"justify"},{"text":"2016 年 10 月，該地區從山壁上掉下一顆約 1、20 噸的大石頭，差一點掉在軌道上。","time":2,"textAlign":"justify"},{"text":"台鐵評估後，決定設置「明隧道」，避免落石直接掉落在軌道上。","time":4,"textAlign":"justify"},{"text":"原本預計於 2020 年 6 月完工，但因為水保及變更設計經四次展延，完工日延至 2021 年 4 月 26 日。","time":6,"textAlign":"justify"},{"text":"不過從 2020 年 3 月以來，無論是台鐵局、交通部各局處在查核時，都有發現缺失。","time":8,"textAlign":"justify"}],"appProps":{"captionsSetting":{"xBoxAlign":"right","xPosition":"8.7%","yBoxAlign":"bottom","yPosition":"20px"},"captionSetting":{"textAlign":"right"},"secondsPer100vh":1.5,"skipLoadLocationRegExp":"editor","forcedPreloadVideo":true,"gsapVersion":"3.5.1","scrollTriggerVersion":"3.5.1","pollingTimeout":700,"preloadCacheType":"force-cache"},"theme":{"mq":{"mobileMaxWidth":"767px"},"captions":{"color":"#fff","link":{"color":"#a67a44","underlineColor":"#a67a44"},"lineHieght":"1.7","mobileLineHeight":"1.7","fontStyle":"normal","fontWeight":"bold","fontSize":"24px","mobile":{"fontSize":"22px"},"fontFamily":"ff-tisa-web-pro, source-han-sans-traditional, Noto Sans TC, PingFang TC, Apple LiGothic Medium, Roboto, Microsoft JhengHei, Lucida Grande, Lucida Sans Unicode, sans-serif","box":{"background":"#404040","width":"450px","mobileWidth":"77%","spanPadding":"6px 15px","mobilePadding":"12px 12px 14px 18px"}}},"uuid":"0bc5857a-5469-4ea1-9ea5-3e565eeffdfd"};
                  window[namespace][pkg].push(data);
                }
              }
            })()
          `,
        },
        {
          hid: 'hide1-2',
          id: 'hide1-2',
          type: 'text/javascript',
          async: true,
          crossOrigin: true,
          body: true,
          src:
            'https://unpkg.com/@twreporter/scrollable-video@1.0.0-rc.3/dist/main.142ef5f0d6d2dfdb8b8d.bundle.js',
        },
      ],
      __dangerouslyDisableSanitizersByTagID: {
        hide1: ['innerHTML'],
      },
    }
  },
  mounted() {
    this.addScrollDetector()
  },
  methods: {
    addScrollDetector() {
      window.onscroll = () => {
        if (
          window.pageYOffset &&
          window.innerHeight + window.pageYOffset >= document.body.offsetHeight
        ) {
          this.$emit('close-video')
        }
      }
    },
  },
}
</script>
