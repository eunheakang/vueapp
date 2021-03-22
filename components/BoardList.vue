<template>
  <div role="tablist">
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-1 variant="info">트로이 여행 후기</b-button>
      </b-card-header>
      <b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <!-- <b-card-text>I start opened because <code>visible</code> is <code>true</code></b-card-text> -->
          <b-card-text>
            <img src='../static/G2.jpg' alt='pic1'/> 
          <!-- <b-img :src="require('../static/G2.jpg')" alt='G2'></b-img> -->
          {{ text }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-2 variant="info">카파도키아 여행 후기</b-button>
      </b-card-header>
      <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>
           <img src='../static/G3.jpg' alt='G3'/>
          {{ text2 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-3 variant="info">파묵칼레 여행 후기</b-button>
      </b-card-header>
      <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>
          <img src='../static/G4.jpg' alt='G4'/>
          {{ text3 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        text: `
          터키어로는 트루바
'트로스의 도시'라는 뜻의 트로이는
그리스 신화의 도시라는사실~
트로이 목마에 대한 신화 이야기를
모르는 분들은 없을것이다!

트로이 역사유적공원으로 조성되어 있어 
입구의 트로이 목마가 포토 스팟!
        `,
        text2: `

벌룬이 그림처럼 예쁜
역사적인 공간도 좋지만 선라이즈
카파도키아는
자연의 신비를 보여줘 더 감동적(♥ω♥*)
새벽 공기를 가르고 열기구 투어가
진행되기 때문에 해 뜰 때만 볼 수 있는
 
떠오르는 열기구와 함께 사진 겟~ 
        `,
        text3: `
         고대 로마시대 상류계층 휴양지 파묵칼레

눈부시게 빛나는 하얀 석회붕은
파란 하늘과 대비되어 눈부신 색감을
보여주는데
파묵칼레에서 잡지의 모델처럼
포즈 잡고 찰-칵
모델 같은 인생샷이을 남겼다✿
        `
      }
    }
  }
</script>