<template>
  <div class="bg">
    <div class="container">



      <v-sheet class="event" elevation='4' color="white">

        <div class="image">
          <img src="poster.png" alt="" class="poster">
        </div>

        <div class="info-block">
          <div class="info-list">
            <v-list disabled id="contacts">
              <v-list-item-group>
                <v-list-item
                  v-for="(item, i) in items"
                  :key="i"
                >
                  <v-list-item-icon>
                    <v-icon v-text="item.icon"></v-icon>
                  </v-list-item-icon>
                  <v-list-item-content>
                    <v-list-item-title v-text="item.text"></v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
              </v-list-item-group>
            </v-list>
          </div>
        </div>

      </v-sheet>

      <v-sheet elevation='4'>
        <script
          type="text/javascript"
          charset="utf-8"
          async
          src="https://api-maps.yandex.ru/services/constructor/1.0/js/?um=constructor%3A550fa481380f6c4fa1db22de0036c972283e8ee9cbe9b48761c5b268f84a9476&amp;width=100%25&amp;height=350&amp;lang=ru_RU&amp;scroll=true">
        </script>
      </v-sheet>

      <v-sheet class="rules" elevation='4' color="white">
        <v-banner>
          <v-avatar
            slot="icon"
            color="deep-purple accent-4"
            size="40"
          >
            <v-icon
              icon="mdi-star"
              color="white"
            >
              mdi-star
            </v-icon>
          </v-avatar>

          <h2>Новости</h2>
        </v-banner>
        </br>

        <p>1-го декабря 2019 года в Сокольниках с большим успехом прошёл уникальный в своем роде Всероссийский Танцевальный Фестиваль "BRUSH". Уникальность этого фестиваля-конкурса в том, что под одной крышей наконец собрались ансамбли бального и социального танца.</p>
        <v-card><v-img  src="media/news/1.jpg" style="float: right;"></v-img></v-card>
        <p>За спортивными состязаниями мы все совсем забыли о красоте бальной хореографии, забыли, что бальный танец является прекрасным выразительным средством, которого так часто хочется видеть на сцене.</p>
        <p>В первом конкурсном дне приняли участие коллективы из Москвы и Московской области.</p>
        <p>Они смогли получить оценку профессионального жюри и услышать мнение действующих тренеров, судей с точки зрения спортивного исполнения и профессионального балетмейстера с точки зрения сценического искусства.</p>

        <p class="font-italic font-weight-bold" style="text-decoration: underline;">Членами жюри стали:</p>
        <v-card><v-img  src="media/news/2.jpg" style="float: right;"></v-img></v-card>
        <ol>
          <li>
            <span class="font-italic font-weight-bold">Димитраш Л. Л.</span></br>
            Педагог-хореограф, постановщик, заслуженный тренер Республики Молдова по спортивно-бальным танцам, судья по спортивно-бальным танцам.
          </li>
          <li>
            <span class="font-italic font-weight-bold">Смирнов Н.Е.</span></br>
            Член Президиума Союза Танцевального спорта Московской области, член образовательного комитета СТСМО, координация работы СТСМО с ВУЗами МО и РФ.</br>
            Мастер спорта по спортивным танцам, чемпион Москвы по европейской программе «Формейшн», финалист открытого чемпионата Европы среди студентов.
          </li>
          <li>
            <span class="font-italic font-weight-bold">Председатель жюри: Бутылкина Е.И.</span></br>
            Балетмейстер- педагог, доцент Российского Гуманитарного Университета им. Косыгина, института «Славянской культуры», кафедры «Педагогика балета». Обладатель гран-при международных фестивалей за балетмейстерские работы.</br>
            Член экспертной Комиссии министерства культуры Московской области. Балетмейстер- постановщик телевизионных и шоу - программ.
          </li>
        </ol>


        <p style="text-decoration: underline;">Первыми победителями и обладателями дипломов ЛАУРЕАТОВ I степени стали:</p>

        <ul>
          <li>Школа танцев <b>«ЭТАЖИ»</b>, рук. Богданова Ольга Олеговна;</li>
          <li>Образцовый Коллектив Бального Танца <b>«КОРРИДА»</b>, рук. Валов Антон Владимирович, Балакина Светлана Владимировна;</li>
          <li>Образцовый коллектив студия бального танца <b>«РАДОНЕЖ»</b>, рук. Пономарева Наталья Владимировна;</li>
          <li>Ансамбль <b>«Грация МГУ»</b>, рук. Лещенко Виталий Анатольевич.</li>
        </ul>

        <p>
          Принято считать, что бальный танец - это парное спортивное танцевание и надо обладать фантазией, опытом и тонким эстетическим вкусом, чтобы средствами бальной хореографии создать грамотный сценический номер. Поэтому организаторами был учреждён кубок за <b style="text-decoration: underline;">ЛУЧШУЮ БАЛЕТМЕЙСТЕРСКУЮ РАБОТУ</b>.
        </p>

        <p>
          Эту особую награду за хореографическую постановку «Марионетки» получила Пономарева Наталья Владимировна руководитель Образцового коллектива студии бального танца «Радонеж» из города Сергиев Посад.
        </p>

        <div class="font-italic font-weight-bold">
          <p>«BRUSH» – это отличная музыка, дружественная атмосфера, потрясающие танцевальные номера.</p>
          <p>Спасибо Всем коллективам и руководителям за такой творческий, теплый зимний вечер!</p>
          <p>Мы очень надеемся, что бальный танец с Вашей помощью наконец станет полноправным участником фестивального движения.</p>
          <p style="text-align: center;">С нетерпением ждём следующих встреч!</p>
        </div>



        <h2>Фото и видеоматериалы с прошедшего фестиваля</h2>
        <p>
          Если вы хотите получить фотографии без водяного знака, напишите номера фотографий нам на почту:
        </p>
        <p>
          <v-icon left>mdi-email</v-icon> brush.festival@gmail.com
        </p>
        <div class="media-cards">
          <div
            v-for="card in cards"
            :key="card.title"
            class="media-item"
          >
            <a :href="card.href" target="_blank">
              <v-card :hover="true">
                <v-img
                  :src="card.src"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="200px"
                >
                  <v-card-title v-text="card.title"></v-card-title>
                </v-img>
              </v-card>
            </a>
          </div>
        </div>
      </v-sheet>

      <v-sheet class="rules" id="rules" elevation='4' color="white">
        <v-banner>
          <v-avatar
            slot="icon"
            color="deep-purple accent-4"
            size="40"
          >
            <v-icon
              icon="mdi-book"
              color="white"
            >
              mdi-book
            </v-icon>
          </v-avatar>

          <h2>Положение</h2>
        </v-banner>

        <h3>ОБЩИЕ ПОЛОЖЕНИЯ:</h3>

        <p>
          Настоящее положение определяет порядок и регламент проведения танцевального фестиваля «BRUSH».
        </p>
        <p>
          Бальный танец стоял всегда особняком в большой семье танцевального
          искусства. Со временем он стал спортивным, а на сегодня вообще потерял своё имя.
          Вернуть статус и величие бального танца в мир хореографического искусства,
          познакомить зрителя с его красотой не только в спортивном зале, но и на сцене – такова
          главная задача Московского областного открытого фестиваля «Brush».
        </p>
        <p>
          Уникальный проект создан при поддержке Центра развития танцевального искусства.
        </p>
        <p>
          Ещё одной актуальной задачей этого фестиваля является максимальное
          привлечение молодёжной аудитории, так как на сегодняшний день в любительских
          танцевальных коллективах (фестивальное движение) основной упор делают на детское
          танцевание, оставляя за бортом подростков от 14 лет и старше.
        </p>
        <p>
          Анализируя работу в этом направление в других регионах страны, были сделаны
          выводы, что в Московской области имея большой потенциал и потребность,
          реализацией этой темы занимаются недостаточно.
        </p>
        <p>
          Главными принципами конкурса являются: открытость, прозрачность критериев
          оценивания, коллегиальность принятия решений, равенство условий для всех
          участников.
        </p>

        <h3>1. ЦЕЛИ И ЗАДАЧИ:</h3>

        <h4>Цели:</h4>
        <ol>
          <li>Развитие творческого потенциала детских танцевальных коллективов бального и социального танцев;</li>
          <li>Знакомство с творчеством и исполнительским мастерством хореографических коллективов разных регионов России;</li>
          <li>Установление творческих контактов, обмен педагогическим опытом работы.</li>
        </ol>

        <h4>Задачи:</h4>
        <ul>
          <li>выявление и демонстрация творческого потенциала детских танцевальных коллективов бального и социального танца;</li>
          <li>развитие и популяризация бального и социального танца в сценическом прочтении;</li>
          <li>создание творческой атмосферы для профессионального общения участников фестиваля, обмена опытом и репертуаром;</li>
          <li>повышение профессионального уровня руководителей коллективов (проведение круглых столов для руководителей);</li>
          <li>объединение и взаимодействие руководителей, преподавателей, педагогов, участников детских и юношеских коллективов.</li>
        </ul>

        <h3>СРОКИ ПРОВЕДЕНИЯ: <i>{{ items[0].text }}</i></h3>
        <h3>МЕСТО ПРОВЕДЕНИЯ: <i>{{ items[1].text }}</i></h3>

        <h3>2. УЧАСТНИКИ ФЕСТИВАЛЯ:</h3>
        <ol>
          <li>В фестивале принимают участи детские, молодёжные и взрослые творческие (танцевальные) коллективы из разных регионов России, представляющие бальную хореографию и социальный танец (независимо от ведомственной принадлежности).</li>
          <li>К участию допускаются коллективы как профессиональные, так и любительские (максимальное количество участников в коллективе не ограничено).</li>
        </ol>

        <h3>3. ВОЗРАСТНЫЕ КАТЕГОРИИ (ГРУППЫ):</h3>
        <ol>
          <li>младшая возрастная категория  (дети-1, дети-2) от 4 до 9 лет</li>
          <li>средняя возрастная категория (юниоры-1) от 10 до 12 лет</li>
          <li>старшая возрастная категория (юниоры-2) от 13 до 15 лет</li>
          <li>молодёжь 16-18 лет</li>
          <li>молодежная возрастная категория (молодежь-2) до 21 года</li>
          <li>взрослые (22 и старше)</li>
        </ol>

        <h3>4. НОМИНАЦИИ КОНКУРСНОЙ ПРОГРАММЫ И КРИТЕРИИ ОЦЕНКИ:</h3>
        <ol>
          <li>Бальные танцевальные номера на основе Европейской и Латиноамериканской программ</li>
          <li>Социальный клубный танец (мамба, бачата, сальса, аргентинское танго и др.);</li>
          <li>Историко-бытовой танец;</li>
          <li>Буги – вуги (социальный танец);</li>
          <li>Танцевальное шоу (сюжетный танец);</li>
          <li>American smooth;</li>
          <li>Секвей;</li>
          <li>Форейшн.</li>
        </ol>

        <h4>Формы (категории):</h4>
        <ul>
          <li>Соло;</li>
          <li>Дуэты;</li>
          <li>Малая форма (от 3-х до 6-ти человек);</li>
          <li>Ансамбли.</li>
        </ul>

        <h4>Критерии оценки:</h4>
        <ul>
          <li>Техника исполнения лексического материала;</li>
          <li>Композиционное построение номера, оригинальность балетмейстерского решения;</li>
          <li>Соответствие репертуара возрастным особенностям исполнителей;</li>
          <li>Подбор и соответствие музыкального материала;</li>
          <li>Артистизм исполнителей и раскрытие художественного образа;</li>
          <li>Соответствие костюма и художественного образа номера.</li>
        </ul>

        <h3>5. ОБЩИЕ ТЕХНИЧЕСКИЕ ТРЕБОВАНИЯ И УСЛОВИЯ УЧАСТИЯ В КОНКУРСЕ:</h3>
        <ol>
          <li>Выступления должны сопровождаться качественной фонограммой, музыкальной композицией, записанной на флеш-носителе в формате «wav» или «МР3» формате. Имейте дубликаты.</li>
          <li>Все фонограммы высылаются по электронной почте в оргкомитет конкурса после внесения оплаты организационного взноса с указанием названия коллектива, названия номера и авторов (исполнителя) музыкального произведения;</li>
          <li>Сопровождающие педагоги, руководители коллективов, родители (опекуны) несут полную ответственность за жизнь и здоровье участников;</li>
          <li>По правилам пожарной безопасности запрещается использовать пожароопасные предметы, в том числе пиротехнику, свечи, факелы, бенгальские огни, декорации и другие предметы, не соответствующие пожарной безопасности.</li>
          <li>Оргкомитет не несёт ответственности за неверно сообщённые или изменённые участником предоставленные сведения.</li>
          <li>Оргкомитет имеет право прекратить приём заявок в любое время, если лимит участников конкурса исчерпан.</li>
        </ol>

        <h3>7. УСЛОВИЯ УЧАСТИЯ:</h3>
        <ol>
          <li>Коллективы (участники) обязаны представить в конкурсной программе два номера.</li>
          <li>Общая продолжительность представленных номеров в каждой номинации не должна превышать 10 мин.</li>
          <li>Общая продолжительность представленных номеров построенных по правилам и требованиям «Формейшн» не должна превышать 12 мин.</li>
        </ol>

        <h3>8. ЖЮРИ ФЕСТИВАЛЯ «BRUSH»:</h3>
        <p>Жюри фестиваля формируется из ведущих специалистов и деятелей культуры и спортивного бального танца, а также ведущих педагогов известнейших ВУЗов.</p>

        <h3>ФИНАНСОВЫЕ УСЛОВИЯ ФЕСТИВАЛЯ</h3>
        <h4>Благотворительный целевой взнос.</h4>

        <ul>
          <li>Соло – 1000 руб. с человека за один номер</li>
          <li>Дуэт – 1000 руб. с человека за один номер</li>
          <li>Малая форма – 800 руб. с человека за один номер</li>
          <li>До 10 человек – 700 руб. с человека за один номер</li>
          <li>Свыше 11 человек – 600 руб. с человека за один номер</li>
          <li>Секвей – 2000 руб. (пара) за один номер</li>
        </ul>

      </br>
        <!-- <v-alert text elevation="4" border="left" color="#6B4791">
          <h4>Акция “Пригласи друзей на Фестиваль”:</h4>

          <p>Условия акции:</p>
          <p>При условии участия Вашего коллектива в данном фестивале вы можете получить дополнительную скидку в 15% для оплаты участия вашего коллектива, а именно Вам необходимо пригласить другие знакомые Вам коллективы для участия в нашем фестивале. Скидку Вы получите при подтверждении участия приглашённых коллективов (заявка + оплата).</p>
        </v-alert> -->

        <h4>ВХОД для зрителей, родителей и сопровождающих лиц БЕСПЛАТНО.</h4>
        </br>

        <v-alert text elevation="4" border="left" type="info">
          <h4>Порядок и сроки подачи заявок:</h4>
          <ul>
            <li>Для подачи заявки, нужно заполнить <a href="https://forms.gle/UKpj82JGUBMz9Kvd6">форму на сайте</a> или отправить заполненный <a href="request.docx">электронный документ</a> на почту <a href="mailto:brush.festival@gmail.com">brush.festival@gmail.com</a></li>
            <li>Заявки принимаются до 20-го апреля (включительно).</li>
          </ul>
        </v-alert>

        <h4>Программа фестиваля будет выслана по факту формирования заявок на электронный адрес.</h4>

        <p>По дополнительным вопросам обращаться по телефону:</p>
        <p>{{ items[3].text }}</p>
        <p>{{ items[4].text }}</p>

      </v-sheet>
    </div>
  </div>
</template>

<script>
  export default {
    data: () => ({
      items: [
        { text: '24 апреля 2021г.', icon: 'mdi-calendar' },
        { text: 'г.Химки, ДК «Родина», Ленинский проспект, 2а', icon: 'mdi-city' },
        { text: 'brush.festival@gmail.com', icon: 'mdi-email' },
        { text: '8 (903) 798-41-02 (Николай Валентинович)', icon: 'mdi-phone' },
        { text: '8 (495) 571-21-58 (офис)', icon: 'mdi-phone' }
      ],
      cards: [
        { title: 'Массовый спорт',
          src: 'media/comp.jpg',
          href: 'https://drive.google.com/open?id=1mlzTl_Xeelg30ez0eA5ppRbY7oFNV7H3',
        },
        { title: 'Ансамбли',
          src: 'media/fest.jpg',
          href: 'https://drive.google.com/open?id=1Ea5WFe0PVunGKnpnNkF2lu4XQ6EbGAvV',
        },
        { title: 'Видео',
          src: 'media/video.jpg',
          href: 'https://www.youtube.com/playlist?list=PLqKyk6IE64I9AIEXIZR_zDXueV-etUtcX',
        },
      ],
    }),
  }
</script>

<style lang="scss" scoped>
  .bg {
    background-color: #eee;
  }
  .container {
    max-width: 960px;
  }
  .media-cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    .media-item {
      width: calc(100% / 3.1);
    }
    a {
      text-decoration: none;
    }
  }
  .event {
    margin: 1em 0 2em;
  }
  .poster {
    display: block;
    width: 100%;
  }
  .info-block {
    width: 100%;
    .v-list-item__title {
      white-space: normal;
    }
  }
  @media (min-width: 500px) {
    .event {
      display: -webkit-flex;
      display: -ms-flex;
      display: flex;
      width: 100%;
    }
    .image {
      flex: 0 0 40%;
    }
    .info-block {
      display: -webkit-flex;
      display: -ms-flex;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      .v-list {
        padding: 0;
      }
    }
  }
  .rules {
    padding: 1em;
    margin: 2em 0 3em;
    h2,
    h3,
    h4,
    ul,
    ol {
      margin-top: .25em;
      margin-bottom: .5em;
    }
    h3 {
      margin-top: 1em;
      margin-bottom: .5em;
    }
  }
  @media (min-width: 500px) {
    .rules {
      padding: 2em;
    }
  }
</style>
