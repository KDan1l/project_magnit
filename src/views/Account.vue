<template>
  <section class="logo">
    <a href="https://magnit.ru/">
      <img class="light-hover" src="img/Лого.svg" alt="logo" />
    </a>
  </section>
  <section class="card">
    <div class="card__employee">
      <a class="light-hover card__employee__table-link" href="">
        <img src="img/right 1.svg" alt="к таблице" class="left-arrow" />
        <p class="card__employee__table-link-text">К таблице</p>
      </a>

      <div class="card__employee__account">
        <img class="card__employee__avatar" src="img/Ава.svg" alt="avatar" />

        <p class="card__employee__account-text">Иванов Андрей Семёнович</p>
        <p class="card__employee__account-text">27 января 1983</p>
        <p class="card__employee__account-text">IvanovAS@gmail.com</p>
        <p class="card__employee__account-text">Отдел маркетинга</p>
        <p class="card__employee__account-text">Начальник отдела</p>

        <button class="card__employee__account__button-exit light-hover">
          Выход
        </button>
      </div>

      <div class="card__wrap"></div>

      <form action="#" method="post" class="card__employee__numbers">
        <div>
          <div
            class="card__employee__numbers__telephone-number"
            v-for="(phone, idx) in phones"
            v-bind:key="idx"
          >
            <input
              type="text"
              name="number"
              class="telephone-number-text"
              placeholder="Введите номер"
              v-model="phones[idx]"
            />

            <img
              class="delete-number__minus light-hover"
              src="img/Минус.svg"
              alt="Удалить номер"
              v-if="idx > 0"
              v-on:click="removeOldPhone(idx)"
            />
          </div>
        </div>

        <!-- <div class="card__employee__numbers__telephone-number">
          <input
            type="text"
            name="number"
            class="telephone-number-text"
            placeholder="Введите номер"
            value="+7 (666) 323-45-23"
          />

          <img
            class="delete-number__minus light-hover"
            src="img/Минус.svg"
            alt="Удалить номер"
          />
        </div> -->

        <div
          class="card__employee__numbers__add-number light-hover"
          v-on:click="addNewPhone"
          v-if="phones.length < 5"
        >
          <img
            src="img/Плюс.svg"
            alt="добавить номер"
            class="add-number__plus"
          />
        </div>

        <div class="card__wrap"></div>

        <button class="card__employee__numbers__button-save light-hover">
          Сохранить
        </button>
      </form>
    </div>
    <div class="card__wrap"></div>
    <p class="card__warning">
      *Для редактирования таблицы перейдите в полную версию сайта
    </p>
  </section>
</template>
<script>
export default {
  data() {
    return {
      phones: [],
    };
  },
  methods: {
    addNewPhone() {
      this.phones.push("");
    },
    removeOldPhone(idx) {
      this.phones.splice(idx, 1);
    },
  },
};
</script>