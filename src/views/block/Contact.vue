<template>
  <section id="contact" class="contact-area py-120">
    <div class="container">
      <div class="justify-center row">
        <div class="w-full mx-4 lg:w-1/2">
          <div class="pb-10 text-center section-title">
            <h4 class="title">Отправьте сообщение</h4>
            <!-- <p class="text">
              Stop wasting time and money designing and managing a website that
              doesn’t get results. Happiness guaranteed!
            </p> -->
          </div>
          <!-- section title -->
        </div>
      </div>
      <!-- row -->
      <div class="justify-center row">
        <div class="w-full lg:w-2/3">
          <div class="contact-form">
            <form
              id="contact-form"
              action="assets/contact.php"
              method="post"
              data-toggle="validator"
            >
              <div class="row">
                <div class="w-full md:w-1/2">
                  <div class="mx-4 mb-6 single-form form-group">
                    <input
                      type="text"
                      name="name"
                      placeholder="Как Вас зовут"
                      data-error="Name is required."
                      required="required"
                    />
                    <div class="help-block with-errors"></div>
                  </div>
                  <!-- single form -->
                </div>
                <div v-if="1==2" class="w-full md:w-1/2">
                  <div class="mx-4 mb-6 single-form form-group">
                    <input
                      type="email"
                      name="email"
                      placeholder="Your Email"
                      data-error="Valid email is required."
                      required="required"
                    />
                    <div class="help-block with-errors"></div>
                  </div>
                  <!-- single form -->
                </div>
                <div v-if="1==2" class="w-full md:w-1/2">
                  <div class="mx-4 mb-6 single-form form-group">
                    <input
                      type="text"
                      name="subject"
                      placeholder="Subject"
                      data-error="Subject is required."
                      required="required"
                    />
                    <div class="help-block with-errors"></div>
                  </div>
                  <!-- single form -->
                </div>
                <div class="w-full md:w-1/2">
                  <div class="mx-4 mb-6 single-form form-group">
                    <input
                      type="text"
                      name="phone"
                      placeholder="Телефон"
                      data-error="Телефон обязателен."
                      required="required"
                    />
                    <div class="help-block with-errors"></div>
                  </div>
                  <!-- single form -->
                </div>
                <div class="w-full">
                  <div class="mx-4 mb-6 single-form form-group">
                    <textarea
                      rows="5"
                      placeholder="Ваше сообщение"
                      name="message"
                      data-error="Пожалуйста, напишите своё сообщение."
                      required="required"
                    ></textarea>
                    <div class="help-block with-errors"></div>
                  </div>
                  <!-- single form -->
                </div>
                <p class="mx-4 form-message"></p>
                <div class="w-full">
                  <div class="mx-4 mt-2 text-center single-form form-group">
                    <button
                      type="submit"
                      class="main-btn gradient-btn focus:outline-none"
                    >
                      Отправить сообщение
                    </button>
                  </div>
                  <!-- single form -->
                </div>
              </div>
              <!-- row -->
            </form>
          </div>
          <!-- row -->
        </div>
      </div>
      <!-- row -->
    </div>
    <!-- container -->
  </section>
</template>

<script>
import { ref } from 'vue'

export default {
  components: {},
  setup() {
    // const menuHidden = ref(true)

    // const speces0 = ref([
    const speces0 = [
      {
        name: 'Андрей Сотников',
        city: 'г.Кострома.',
        opis:
          'Энергопрактик. Шаман. Гипнолог. Специалист по работе с картами ТАРО.  С помощью специальных практик открывает нужные энергитические каналы',
        img: 'mimQlW4Oi0c.jpg',
      },
      {
        name: 'Камиль Зияев',
        city: 'г.Санкт-Петербург',
        opis: 'Костоправ. Массажист. Гипнолог. Специалист широкого профиля',
        img: '2c07AnT8xio.jpg',
      },
      {
        name: 'Алексей Корнев',
        city: 'г.Кострома',
        opis:
          'Массажист. Гипнолог. Энергопрактик. Словами лечит душу, рукамилечит тело.',
        img: 'UIfxrJ_G_jw.jpg',
      },
      {
        name: 'Олег Баранов',
        city: 'Москва',
        opis: 'Гипнотизёр. Мастер директивного гипноза. Семейный психолог.',
        img: 'I40FVh7KHDo.jpg',
      },
      {
        name: 'Клавдия Жуковская',
        city: 'г. Москва',
        opis: 'Ментальный психолог. Энерготерапевт. Целитель.',
        img: 'bWk3SJP39VM.jpg',
      },
      {
        name: 'Олеся Шаламова',
        city: 'г. Тольятти',
        opis: 'Гипнолог. Шаманка. Мастер висцерального массажа.',
        img: 'uYe8VwKrd4o.jpg',
      },
      {
        name: 'Татьяна Колданова',
        city: '',
        opis: 'Семейный психолог. Гипнолог. Мастер Эриксоновского гипноза.',
        img: 'JGzibqTDPGk.jpg',
      },
      {
        name: 'Михаил Эджибов',
        city: 'г. Санкт-Петербург',
        opis: 'Психолог. Регресолог. Гипнолог. Художник.',
        img: 'Fs_c_dMotes.jpg',
      },
      {
        name: 'Таисия Комова',
        city: 'г. Омск',
        opis: 'Регресолок, Нумеролог, Эзотерик, Гипнолог.',
        img: 'Rg-FiavZvag.jpg',
      },
      {
        name: 'Зинаида Блажко',
        city: 'г. Москва',
        opis: 'Энергопрактик. Семейный психолог. Гипнолог. Дизайнер.',
        img: 'HsK5pV9wYAg.jpg',
      },
      {
        name: 'Дарья Пыжив',
        city: 'г. Евпатория',
        opis: 'Духовный наставник. Гипнолог. Ведьма.',
        img: 'T996viIyVGI.jpg',
      },
      {
        name: 'Алексей Шестаков',
        city: 'г. Екатеренбург',
        opis: 'Нарколог. Гипнолог. за один сеанс убирает влечение к алкоголю',
        img: 'LU16_l4QePs.jpg',
      },
      // ])
    ]

    // const speces = ref( speces0.value.sort((a,b) => Math.random() - 0.5) )
    const speces = speces0.sort((a, b) => Math.random() - 0.5)

    return {
      // menuHidden,
      speces,
    }
  },
}
</script>

<style>
.growing-underline {
  display: block;
  position: relative;
  padding: 0.2em 0;
  overflow: hidden;
}

.growing-underline::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 0.1em;
  background-color: black;
  transition: opacity 300ms, transform 300ms;
  opacity: 1;
  transform: translate3d(-100%, 0, 0);
}

.growing-underline:hover::after,
.growing-underline:focus::after {
  transform: translate3d(0, 0, 0);
}
</style>
