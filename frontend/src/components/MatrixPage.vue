<template>
  <div class="main_page">
    <div class="header">
      <div class="header_container">
        <img src="../../img/logo.svg" alt="">
        <p class="header_text">Nickname</p>
      </div>
      <div class="balance_container">
        <p class="balance">Пополнить</p>
      </div>
    </div>
    <div class="ref">
      <p class="ref_balance">200 руб</p>
    </div>
    <p class="head_text">Введите дату рождения</p>
    <div class="main_head">
      <SelectPage
      :options="['1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12', '13', '14', '15', '16', '17', '18', '19', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31']"
      @input="option => selectedTimeZone = option"
      :placeholderdata="'Число'"
      />
      <SelectPage
      :options="['Январь', 'Февраль', 'Март', 'Апрель', 'Май', 'Июнь', 'Июль', 'Август', 'Сентябрь', 'Октябрь', 'Ноябрь', 'Декабрь']"
      @input="option => selectedTimeZone = option"
      :placeholderdata="'Месяц'"
      />
      <SelectPage
      :options="['1950', '1951', '1952', '1953', '1954', '1955', '1956', '1957', '1958', '1959', '1960', '1961', '1962', '1963', '1964', '1965', '1966', '1967', '1968', '1969', '1970', '1971', '1972', '1973', '1974', '1975', '1976', '1977', '1978', '1979', '1980', '1981', '1982', '1983', '1984', '1985', '1986', '1987', '1988', '1989', '1990', '1991', '1992', '1993', '1994', '1995', '1996', '1997', '1998', '1999', '2000', '2001', '2002', '2003', '2004', '2005', '2006', '2007', '2008', '2009', '2010', '2011', '2012', '2013', '2014', '2015', '2016', '2017', '2018', '2019', '2020', '2021', '2022', '2023', '2024']"
      @input="option => selectedTimeZone = option"
      :placeholderdata="'Год'"
      />  
    </div>
    <button class="calculation">Рассчитать</button>
    <img src="../../img/Matrix.png" alt="" class="matrix_img">
    <p class="heart_text">Карта здоровья</p>
    <table width="100%" border="0" cellspacing="2" class="tabl">
      <tbody><tr style=" font-size:12px; font-weight:bold;">
          <td style="background:#f4f4f6;" align="center" valign="middle">НАЗВАНИЕ ЧАКРЫ</td>
          <td style="background:#f4f4f6;" align="center" valign="middle">ФИЗИКА</td>
          <td style="background:#f4f4f6;" align="center" valign="middle">ЭНЕРГИЯ</td>
          <td style="background:#f4f4f6;" align="center" valign="middle">ЭМОЦИИ</td>
      </tr>
      <tr style=" color:#FFFFFF;">
          <td class="trans" id="chakra7" style="background:#993399; " align="center" valign="middle"><span class="td_chakra">Сахасрара</span></td>
          <td style="background:#993399; " class="trans" id="n33" align="center" valign="middle">7</td>
          <td style="background:#993399; " class="trans" id="n34" align="center" valign="middle">5</td>
          <td style="background:#993399; " class="trans" id="n35" align="center" valign="middle">12</td>
      </tr>
      <tr style=" color:#FFFFFF;">
          <td class="trans" id="chakra6" style="background:#3366ff;" align="center" valign="middle"><span class="td_chakra">Аджна</span></td>
          <td style="background:#3366ff;" class="trans" id="n36" align="center" valign="middle">5</td>
          <td style="background:#3366ff;" class="trans" id="n37" align="center" valign="middle">19</td>
          <td style="background:#3366ff;" class="trans" id="n38" align="center" valign="middle">6</td>
      </tr>
      <tr style=" color:#FFFFFF;">
          <td class="trans" id="chakra5" style="background:#33ccff;" align="center" valign="middle"><span class="td_chakra">Вишудха</span></td>
          <td style="background:#33ccff;" class="trans" id="n39" align="center" valign="middle">16</td>
          <td style="background:#33ccff;" class="trans" id="n40" align="center" valign="middle">14</td>
          <td style="background:#33ccff;" class="trans" id="n41" align="center" valign="middle">3</td>
      </tr>
      <tr style=" color:#FFFFFF;">
          <td class="trans" id="chakra4" style="background:#66cc66;" align="center" valign="middle"><span class="td_chakra">Анахата</span></td>
          <td style="background:#66cc66;" class="trans" id="n42" align="center" valign="middle">7</td>
          <td style="background:#66cc66;" class="trans" id="n43" align="center" valign="middle">5</td>
          <td style="background:#66cc66;" class="trans" id="n44" align="center" valign="middle">12</td>
      </tr>
      <tr>
          <td class="trans" id="chakra3" style="background:#ffff99" align="center" valign="middle"><span class="td_chakra">Манипура</span></td>
          <td style="background:#ffff99" class="trans" id="n45" align="center" valign="middle">9</td>
          <td style="background:#ffff99" class="trans" id="n46" align="center" valign="middle">9</td>
          <td style="background:#ffff99" class="trans" id="n47" align="center" valign="middle">18</td>
      </tr>
      <tr style="color:#FFFFFF;">
          <td class="trans" id="chakra2" style="background:#ff9900;" align="center" valign="middle"><span class="td_chakra">Свадхистана</span></td>
          <td style="background:#ff9900;" class="trans" id="n48" align="center" valign="middle">15</td>
          <td style="background:#ff9900;" class="trans" id="n49" align="center" valign="middle">9</td>
          <td style="background:#ff9900;" class="trans" id="n50" align="center" valign="middle">6</td>
      </tr>
      <tr style=" color:#FFFFFF;">
          <td class="trans" id="chakra1" style="background:#cc3333;" align="center" valign="middle"><span class="td_chakra">Муладхара</span></td>
          <td style="background:#cc3333;" class="trans" id="n51" align="center" valign="middle">6</td>
          <td style="background:#cc3333;" class="trans" id="n52" align="center" valign="middle">18</td>
          <td style="background:#cc3333;" class="trans" id="n53" align="center" valign="middle">6</td>
      </tr>
      <tr style=" font-weight:bold;">
          <td class="trans" id="chakra" style="background:#cccccc;" align="center" valign="middle"><span class="td_chakra">ИТОГО</span></td>
          <td style="background:#cccccc;" class="trans" id="n54" align="center" valign="middle">11</td>
          <td style="background:#cccccc;" class="trans" id="n55" align="center" valign="middle">16</td>
          <td style="background:#cccccc;" class="trans" id="n56" align="center" valign="middle">9</td>
      </tr>
    </tbody></table>
      <div class="search">
        <p class="search_head">Поиск себя:</p>
        <p class="search_subhead">Соединение мужского и женского. Выстраивание взаимоотношений. Способности, навыки, умения.</p>
      </div>
      <div class="priroda">
        <div class="priroda_cont">
          <p class="priroda_text">Небо:</p>
          <p class="priroda_text">Земля:</p>
        </div>
        <div class="priroda_circle">
          <div class="circles">
            <p class="circle_number">1</p>
          </div>
          <div class="circles">
            <p class="circle_number">1</p>
          </div>
        </div>
        <img src="../../img/path-lines.svg" alt="" class="">
        <div class="circles">
          <p class="circle_number">1</p>
        </div>
      </div>
      <div class="social">
        <p class="social_head">Социализация:</p>
        <p class="social_subhead">Социальная и родовая системы. Результаты и признание в социуме</p>
      </div>
      <div class="priroda">
        <div class="priroda_cont">
          <p class="priroda_text">М:</p>
          <p class="priroda_text">Ж:</p>
        </div>
        <div class="priroda_circle">
          <div class="circles">
            <p class="circle_number">1</p>
          </div>
          <div class="circles">
            <p class="circle_number">1</p>
          </div>
        </div>
        <img src="../../img/path-lines.svg" alt="" class="">
        <div class="circles">
          <p class="circle_number">1</p>
        </div>
      </div>
    <div class="bottom_wrap">
      <div class="wrap-left">
        <p class="search_head">Духовная гармония:</p>
        <div class="circles">
          <p class="circle_number">15</p>
        </div>
      </div>
      <p class="search_subhead">Духовный зачет. Кто я для бога?<br> Где божественное во мне?</p>
    </div>
    <div class="bottom_wrap">
      <div class="wrap-left">
        <p class="search_head">Планетарное:</p>
        <div class="circles">
          <p class="circle_number">15</p>
        </div>
      </div>
      <p class="search_subhead">Планетарное предназначение человека</p>
    </div>
    <p class="transcript"> Расшифровка значений вашей<br>Матрицы судьбы</p>
    <div class="transcript_container">
      <div class="transcript_cards">
        <p class="transcript_text">Визитная карточка</p>
      </div>
      <div class="transcript_cards">
        <p class="transcript_text">Карма прошлого воплощения</p>
      </div>
      <div class="transcript_cards_lock">
        <p class="transcript_text">Главная проработка души</p>
      </div>
      <div class="transcript_cards_lock">
        <p class="transcript_text">Задачи души до 40 лет</p>
      </div>
      <div class="transcript_cards_lock">
        <p class="transcript_text">Отношения</p>
      </div>
      <div class="transcript_cards_lock">
        <p class="transcript_text">Деньги</p>
      </div>
      <div class="transcript_cards">
        <p class="transcript_text">Точка душевного комфорта</p>
      </div>
      <div class="transcript_cards">
        <p class="transcript_text">Родовые задачи</p>
      </div>
      <div class="transcript_cards_lock">
        <p class="transcript_text">Таланты</p>
      </div>
      <div class="transcript_cards">
        <p class="transcript_text">Детско-родительские отношения</p>
      </div>
      <div class="transcript_cards_lock">
        <p class="transcript_text">Предназначение</p>
      </div>
      <div class="transcript_cards">
        <p class="transcript_text">Персональный прогноз по годам</p>
      </div>
      <div class="transcript_cards_lock">
        <p class="transcript_text">Сексуальность</p>
      </div>
    </div>
  </div>
</template>

<script>
import SelectPage from '../components/SelectPage.vue';
export default {
  components: { SelectPage },
  data() {
      return {
          
      }
  },

}
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.header_container {
  display: flex;
  align-items: center;
  gap: 8px;
}
.header_text {
  font-family: Mulish Regular;
  font-size: 28px;
  line-height: 42px;
  text-align: left;
  color: #FFFFFF;
}
.balance_container {
  background: rgba( 23, 33, 43, 0.25 );
  box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
  backdrop-filter: blur( 4px );
  -webkit-backdrop-filter: blur( 4px );
  border-radius: 10px;
  border: 1px solid rgba( 255, 255, 255, 0.18 );
  border-radius: 25px;
  display: flex;
  align-items: center;
  padding: 12px 15px;
}
.balance {
  font-family: Mulish Regular;
  font-size: 20px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #FFFFFF;
}
.ref {
  display: flex;
  justify-content: end;
  align-items: center;
}
.ref_balance {
  font-family: Mulish Regular;
  font-size: 24px;
  line-height: 36px;
  text-align: left;
  color: #FFFFFF;
}
.main_page {
  display: flex;
  flex-direction: column;
  gap: 20px;
}
.main_head{
  display: flex;
  gap: 20px;
}
.head_text{
  font-family: Mulish Regular;
  font-size: 28px;
  line-height: 42px;
  letter-spacing: 0.01em;
  text-align: center;
  color: #FFFFFF;
}
p{
  margin: 0;
}
button {
  color: #FFFFFF;
  background:#6266EA;
  border: none;
  cursor: pointer;
  display: flex;
  height: 36px;
  padding: 10px 14px;
  justify-content: center;
  align-items: center;
  gap: 5px;
  border-radius: 3px;
  transition: all .2s ease;
  font-family: "TT Norms Medium";
}
.matrix_img{
  border-radius: 10px;
}
.tabl td {
  padding: 10px 5px;
}
.search_head{
  font-family: Mulish Semibold;
  font-size: 30px;
  line-height: 42px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #FFFFFF;
}
.search_subhead{
  font-family: Mulish Regular;
  font-size: 16px;
  font-weight: 500;
  line-height: 24px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #FFFFFF;
}
.social_head{
  font-family: Mulish Semibold;
  font-size: 30px;
  line-height: 42px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #FFFFFF;
}
.social_subhead{
  font-family: Mulish Regular;
  font-size: 16px;
  font-weight: 500;
  line-height: 24px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #FFFFFF;
}
.search{
  display: flex;
  flex-direction: column;
  gap: 5px;
  max-width: 300px;
}
.social{
  display: flex;
  flex-direction: column;
  gap: 5px;
  max-width: 300px;
}
.priroda_cont{
  display: flex;
  flex-direction: column;
  gap: 30px;
}
.priroda_text{
  font-family: Mulish Regular;
  font-size: 24px;
  font-weight: 500;
  line-height: 16px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #FFFFFF;
}
.priroda_circle{
  display: flex;
  flex-direction: column;
  gap: 5px;
}
.circles{
  display: flex;
  border: 2px #FFFFFF solid;
  border-radius: 50%;
  height: 36px;
  justify-content: center;
  width: 36px;
  align-items: center;
}
.priroda{
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 15px;
}
.wrap-left{
  display: flex;
  gap: 15px;
}
.bottom_wrap{
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.circle_number{
  color: #FFFFFF;
}
.transcript{
  font-family: Mulish Semibold;
  font-size: 24px;
  color: #FFFFFF;
  text-align: left;
}
.transcript_text{
  color: #000;
  font-family: Mulish Regular;
  text-align: left;
}
.transcript_container{
  display: flex;
  flex-direction: column;
  gap: 15px;
}
.transcript_cards_lock{
  background: #FFFFFF url('../../img/lock.svg') no-repeat right 5px center;
  border-radius: 5px;
  padding: 15px;
}
.transcript_cards{
  background: #FFFFFF url('../../img/next_arrow.png') no-repeat right 5px center;
  border-radius: 5px;
  padding: 15px;
}
.heart_text{
  font-family: Mulish Semibold;
  color: #FFFFFF;
  text-align: left;
  font-size: 30px;
}
td {
  font-family: Mulish Regular;  
}
.calculation{
  font-family: Mulish Semibold;
  font-size: 20px;
}
</style>