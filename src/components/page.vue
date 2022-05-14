<template>
  <div>
    <!-- section : 고수들의 투자 비법 -->
    <section class="invest-section">
      <div class="section-header">
        <h2>고수들의 투자 비법!</h2>
        <a href="javascript:;" class="btn-more">더보기</a>
      </div>
      <div class="section-content">
        <ul class="card-list">
          <li>
              <a href="javascript:;" class="column">
                <span class="category domestic-stock">국내증시동향</span>
                <span class="title">글로벌 부동산 메가 트렌드, 단독주택(Single-Family Raental) 투자</span>
              </a>
              <a href="javascript:;" class="author">
                <span class="author-thumb">
                  <img  src="@/assets/images/sample/sample_author_1.png" />
                </span>
                <span class="author-name">
                  <span>뉴히어로</span>
                  <span class="original">original</span>
                </span>
              </a>
          </li>
          <li>
              <a href="javascript:;" class="column">
                <span class="category invest">투자트랜드</span>
                <span class="title">하락장에 강한 8% 고배당+월배당 ETF 'NUSI'</span>
              </a>
              <a href="javascript:;" class="author">
                <span class="author-thumb">
                  <img  src="@/assets/images/sample/sample_author_1.png" />
                </span>
                <span class="author-name">
                  <span>제이형코치</span>
                  <span class="original">original</span>
                </span>
              </a>
          </li>
          <li>
              <a href="javascript:;" class="column">
                <span class="category overseas-stock">해외증시동향</span>
                <span class="title">인기 걸그룹 빌리, 메타버스 세상 '이프랜드'에 뜬다</span>
              </a>
              <a href="javascript:;" class="author">
                <span class="author-thumb">
                  <img  src="@/assets/images/sample/sample_author_1.png" />
                </span>
                <span class="author-name">
                  <span>부로마블</span>
                  <span class="original">original</span>
                </span>
              </a>
          </li>
        </ul>
      </div>
    </section>
    <!-- // section : 고수들의 투자 비법 -->
    <!-- section : 이번주 꼭 확인하세요! -->
    <section class="week-info-section">
      <div class="section-header">
        <h2>이번주 꼭 확인하세요!</h2>
        <ul class="week-tab-area">
          <li>
            <button type="button" class="active">
              <span class="day-name">월</span>
              <span class="day-num">16</span>
            </button>
          </li>
          <li>
            <button type="button">
              <span class="day-name">화</span>
              <span class="day-num">17</span>
            </button>
          </li>
          <li>
            <button type="button">
              <span class="day-name">수</span>
              <span class="day-num">18</span>
            </button>
          </li>
          <li>
            <button type="button">
              <span class="day-name">목</span>
              <span class="day-num">19</span>
            </button>
          </li>
          <li>
            <button type="button">
              <span class="day-name">금</span>
              <span class="day-num">20</span>
            </button>
          </li>
          <li>
            <button type="button">
              <span class="day-name">토</span>
              <span class="day-num">21</span>
            </button>
          </li>
          <li>
            <button type="button">
              <span class="day-name">일</span>
              <span class="day-num">22</span>
            </button>
          </li>
        </ul>
      </div>
      <div class="section-content">
        <weekInfoList :data="weekData"></weekInfoList>
      </div>
    </section>
    <!-- // section : 이번주 꼭 확인하셍! -->
  </div>
</template>

<script>
import weekInfoList from '@/components/list.vue'

export default {
  name: 'viewPage',
  conponents : {
    weekInfoList
  },
  data() {
    return {
      weekData: [{
        date: '월 5.16',
        list: [{
          category: '상장예정',
          company: 'LG유플러스',
          market: 'KOSDAQ',
          price: '1,234,000',
          supervision: '미래에셋증권',
          period: '22.3.14 - 22.3.15',
          relase: '22.03.14'
        }]    
      }, {
        date: '화 5.17',
        list: [{
          category: '실적',
          company: '롯데제과',
          market: 'KOSDAQ',
          price: '33,350',
          perfomance: '+23%',
          profit: '742억',
          sales: '5180억'
        },{
          category: '이벤트',
          title: '구글 연례 개발자 회의 및 픽셀워치 공개',
          text: '픽셀워치는 구글과 삼성이 공동 개발한 웨어러블용 운용체계(OS) "웨어OS"로 구동되며, 자체 개발한 시스템온칩(Soc)를 탑재할 것으로 알려짐'
        }]
      },{
        date: '수 5.18',
        list: [{
          category: '공모청약',
          company: 'LG 에너지 솔루션',
          market: 'KOSDAQ',
          price: '1,234,000',
          supervision: '신한금융투자',
          period: '22.3.14 - 22.3.15',
          relase: '22.03.14'
        }]  
      },{
        date: '목 5.19',
        list: [{
          category: '실적',
          company: '스튜디오 드래곤',
          market: 'KOSDAQ',
          price: '18,460',
          perfomance: '-23%',
          profit: '247억',
          sales: '3,933억'
        },{
          category: '공모청약',
          company: 'LG 에너지 솔루션',
          market: 'KOSDAQ',
          price: '1,234,000',
          supervision: '신한금융투자',
          period: '22.3.14 - 22.3.15',
          relase: '22.03.14'
        }]  
      },{
        date: '금 5.20',
        list: [{
          category: '이벤트',
          title: 'xEV 트렌드 코리아 개최',
          text: '인터배터리는 국내 유일의 배터리 전문 전시회로 올해 행사에는 국내외 270여개 배터리 산업 관련 기업들이 참가해 새로운 제품과 기술을 선보일 것으로 알려짐'
        }]
      }]
    }
  }
}
</script>

<style scoped>
</style>
