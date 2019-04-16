<template>
  <section class="concerts">
    <div class="concerts__inner">
      <ul class="concerts__list">
        <li class="concerts__item" v-for="(concert, index) in concerts" :key="index">
          <a class="concerts__link" v-bind:class="{'concerts__link--critical': concert.isCritical }" v-bind:href="concert.link">
            <span class="concerts__date">{{ concert.date }}</span>
            <span class="concerts__caption">{{ concert.caption }}</span>
          </a>
        </li>
        <!-- <li class="concerts__item">
          <span class="concerts__note">СПИСОК ГОРОДОВ БУДЕТ ПОПОЛНЯТЬСЯ</span>
        </li> -->
      </ul>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'Concerts',
    data: function () {
      return {
        concerts: [
          {
            link: 'https://vk.com/flesh_cheb21',
            date: '08.12',
            caption: 'ЧЕБОКСАРЫ'
          },
          {
            link: 'https://vk.com/flesh_vnov',
            date: '12.12',
            caption: 'В. НОВГОРОД'
          },
          {
            link: 'https://vk.com/flesh_pskov',
            date: '13.12',
            caption: 'ПСКОВ'
          },
          {
            link: 'https://vk.com/flesh_smolensk',
            date: '14.12',
            caption: 'СМОЛЕНСК'
          },
          {
            link: 'https://vk.com/flesh_bryansk',
            date: '15.12',
            caption: 'БРЯНСК'
          },
          {
            link: 'https://vk.com/flesh_orel',
            date: '16.12',
            caption: 'ОРЁЛ'
          },
          {
            link: 'https://vk.com/flesh_penza',
            date: '18.12',
            caption: 'ПЕНЗА'
          },
          {
            link: 'https://vk.com/flesh_tambov',
            date: '19.12',
            caption: 'ТАМБОВ'
          },
          {
            link: 'https://vk.com/flesh_lipetsk',
            date: '20.12',
            caption: 'ЛИПЕЦК'
          },
          {
            link: 'https://vk.com/flesh_whitecity',
            date: '21.12',
            caption: 'БЕЛГОРОД'
          },
          {
            link: 'https://vk.com/flesh_voron',
            date: '22.12',
            caption: 'ВОРОНЕЖ'
          },
          {
            link: 'https://vk.com/flesh_kursk',
            date: '23.12',
            caption: 'КУРСК'
          },
          {
            link: 'https://vk.com/flesh__samara',
            date: '30.01',
            caption: 'САМАРА'
          },
          {
            link: 'https://vk.com/fleshufa',
            date: '31.01',
            caption: 'УФА'
          },
          {
            link: 'https://vk.com/flesh_ekb_2019',
            date: '02.02',
            caption: 'ЕКАТЕРИНБУРГ',
            isCritical: true
          },
          {
            link: 'https://vk.com/fleshhbk',
            date: '07.02',
            caption: 'ХАБАРОВСК'
          },
          {
            link: 'https://vk.com/fleshvladivostok2019',
            date: '08.02',
            caption: 'ВЛАДИВОСТОК'
          },
          {
            link: 'https://vk.com/flesh_irkutsk',
            date: '09.02',
            caption: 'ИРКУТСК'
          },
          {
            link: 'https://vk.com/flesh_uu',
            date: '10.02',
            caption: 'УЛАН-УДЭ'
          },
          {
            link: 'https://vk.com/flesh_brnl',
            date: '13.02',
            caption: 'БАРНАУЛ'
          },
          {
            link: 'https://vk.com/fleshnsk',
            date: '14.02',
            caption: 'НОВОСИБИРСК'
          },
          {
            link: 'https://vk.com/flesh_kmrv',
            date: '15.02',
            caption: 'КЕМЕРОВО'
          },
          {
            link: 'https://vk.com/flesh_tmsk',
            date: '16.02',
            caption: 'ТОМСК'
          },
          {
            link: 'https://vk.com/flesh_krsk_2019',
            date: '17.02',
            caption: 'КРАСНОЯРСК'
          },
          {
            link: 'https://vk.com/flesh_mrm',
            date: '20.02',
            caption: 'МУРМАНСК'
          },
          {
            link: 'https://vk.com/flesh_astr',
            date: '25.02',
            caption: 'АСТРАХАНЬ'
          },
          {
            link: 'https://vk.com/flesh_volg',
            date: '26.02',
            caption: 'ВОЛГОГРАД'
          },
          // {
          //   link: 'https://vk.com/flesh_kzn',
          //   date: '01.03',
          //   caption: 'КАЗАНЬ'
          // },
          {
            link: 'https://vk.com/fleshkirov',
            date: '02.03',
            caption: 'КИРОВ'
          },
          {
            link: 'https://vk.com/fleshnn',
            date: '03.03',
            caption: 'Н.НОВГОРОД'
          },
          {
            link: 'https://vk.com/flesh_kaluga',
            date: '11.03',
            caption: 'КАЛУГА'
          },
          {
            link: 'https://vk.com/flesh_tula',
            date: '12.03',
            caption: 'ТУЛА'
          },
          {
            link: 'https://vk.com/flesh_ryazan',
            date: '13.03',
            caption: 'РЯЗАНЬ'
          },
          {
            link: 'https://vk.com/flesh_vladimir',
            date: '14.03',
            caption: 'ВЛАДИМИР'
          },
          {
            link: 'https://vk.com/flesh_ivan',
            date: '15.03',
            caption: 'ИВАНОВО'
          },
          {
            link: 'https://vk.com/flesh_tver',
            date: '16.03',
            caption: 'ТВЕРЬ'
          },
          {
            link: 'https://vk.com/flesh_saratov',
            date: '17.03',
            caption: 'САРАТОВ'
          },
          {
            link: 'https://vk.com/flesh_72',
            date: '20.03',
            caption: 'ТЮМЕНЬ'
          },
          {
            link: 'https://vk.com/fleshkrd',
            date: '22.03',
            caption: 'КРАСНОДАР'
          },
          {
            link: 'https://vk.com/fleshrnd',
            date: '23.03',
            caption: 'РОСТОВ'
          },
          {
            link: 'https://vk.com/fleshsochi',
            date: '30.03',
            caption: 'СОЧИ'
          },
        ]
      }
    }
  }
</script>

<style>
  .concerts {
    
  }

  .concerts__inner {
    width: 350px;
    margin: 0 auto;
  }

  .concerts__list {
    list-style: none;
    margin: 0;
    padding: 0;
  }

  .concerts__item {
    cursor: pointer;
    margin-bottom: 15px;
  }

  .concerts__link {
    text-decoration: none;
    font-size: 30px;
    letter-spacing: 3px;
    color: #fdb56b;
    display: flex;
    justify-content: space-between;
    transition: 0.2s all;
    text-shadow: 1px 1px 2px black, 0 0 1em black;
  }

  .concerts__link:hover,
  .concerts__link:focus {
    color: #cf3131;
  }

  .concerts__link--critical {
    color: #cf3131;
  }

  .concerts__link--critical:hover,
  .concerts__link--critical:focus {
    color: #fdb56b;
  }

  .concerts__date {
    display: inline-block;
    margin-right: 20px;
  }

  .concerts__caption {
    display: inline-block;
  }

  .concerts__note {
    color: #cf3131;
    font-size: 30px;
    display: inline-block;
    padding-top: 20px;
    text-shadow: 1px 1px 2px black, 0 0 1em black;
  }

  @media (max-width: 1280px) and (min-width: 769px) {
    .concerts__inner {
      width: 300px;
    }

    .concerts__link {
      font-size: 24px;
    }
  }

  @media (max-width: 768px) {
    .concerts__inner {
      width: 300px;
    }

    .concerts__link {
      font-size: 20px;
    }
  }

</style>
