<template>
  <nav class="nav">
    <ul class="nav__list">
      <li class="nav__list__item">
        <a class="light-hover nav-text" href="#">Администратор</a>
      </li>
      <li class="nav__list__item">
        <a class="light-hover nav-text" href="#">
          <div class="nav__list__item__account light-hover">
            <p class="nav-text">Вадим Геннадьевич Колпак</p>
            <img
              src="img/table__avatar.svg"
              alt="Фото профиля"
              class="nav__list__item__account__avatar"
            />
            <img
              src="img/table__Vector 1.svg"
              alt="Развернуть список"
              class="nav__list__item__account__narrow"
            />
          </div>
        </a>
        <div class="nav__list__togler">
          <p class="nav__list__togler__item">
            <a class="light-hover nav-text" href="./account">Личный кабинет</a>
          </p>
          <p class="nav__list__togler__item">
            <a class="light-hover nav-text" href="#">Выход</a>
          </p>
        </div>
      </li>
    </ul>
  </nav>

  <section class="main">
    <div class="main__menu">
      <form class="main__menu__form" action="">
        <div class="main__menu__form__btns">
          <button class="main__menu__form__btn btn-save">
            <img src="img/table__save.svg" alt="сохранить изменения" />
          </button>
          <button class="main__menu__form__btn btn-export">
            <img
              src="img/table__export_delivery-box 1.svg"
              alt="экспортировать таблицу"
            />
          </button>
          <button class="main__menu__form__btn btn-add">
            <img
              src="img/table__add-user 1.svg"
              alt="Добавить запись о сотруднике"
            />
          </button>
        </div>
        <div class="main__menu__form__search">
          <input
            class="main__menu__form__search__input"
            name="search"
            type="text"
            placeholder="Поиск..."
          />

          <div class="flex-right">
            <select class="main__menu__form__search__category light-hover">
              <option class="option">Искать везде</option>
              <option class="option">Его идеи</option>
              <option class="option">Где он?</option>
            </select>
            <button class="main__menu__form__btn-search light-hover">
              <img
                class="main__menu__form__btn-search-img"
                src="img/table__search-loupe 1.svg"
                alt="Искать"
              />
            </button>
          </div>
        </div>
      </form>
    </div>

    <div class="table__background-logo">
      <div class="table__background-shadows">
        <div class="main__table">
          <table class="content-table">
            <thead>
              <tr>
                <td>
                  <div class="content-table__name-and-button">
                    <p class="content-table__name">ФИО</p>
                    <form class="content-table__formn">
                      <button class="content-table__form__button">
                        <img
                          class="content-table__button__arrow"
                          src="img/table__Vector 1.svg"
                          alt="упорядочить"
                        />
                      </button>
                    </form>
                  </div>
                </td>
                <td>Номера телефонов</td>
                <td>Эл. Почта</td>
                <td>Подразделение</td>
                <td>должность</td>
                <td>Дата обновления</td>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>1. Петров Василий Борисович</td>
                <td>
                  <p class="table__number">+7(960) 234-19-91</p>
                </td>
                <td>Petrov1983@mail.ru</td>
                <td>Маркетинг</td>
                <td>Начальник отдела</td>
                <td>27 февраля 2021</td>
              </tr>
              <tr>
                <td>2. Сидоров Петр Петрович</td>
                <td>
                  <p class="table__number">+7(960) 591-49-57</p>
                  <p class="table__number">567-29-31</p>
                </td>
                <td>SidorovPP@gmail.ru</td>
                <td>Маркетинг</td>
                <td>Старший аналитик</td>
                <td>18 февраля 2020</td>
              </tr>
              <tr>
                <td>3. Смирнов Игорь Андреевич</td>
                <td>
                  <p class="table__number">+7(978) 154-22-99</p>
                </td>
                <td>Smirnov19@mail.ru</td>
                <td>Маркетинг</td>
                <td>Аналитик</td>
                <td>9 октября 2019</td>
              </tr>
              <tr>
                <td>4. Андреев Андрей Аристархович</td>
                <td>
                  <p class="table__number">+7(960) 978-56-81</p>
                  <p class="table__number">+7(978) 222-15-31</p>
                  <p class="table__number">617-12-41</p>
                </td>
                <td>AndreevAA@mail.ru</td>
                <td>Маркетинг</td>
                <td>Аналитик</td>
                <td>1 июня 2020</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </section>
</template>