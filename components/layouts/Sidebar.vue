<template>
  <div>
    <div class="main-sidebar sidebar-style-2">
      <aside id="sidebar-wrapper">
        <div class="sidebar-brand">
          <nuxt-link to="/">Nuxt Stisla</nuxt-link>
        </div>
        <div class="sidebar-brand sidebar-brand-sm">
          <nuxt-link to="/">Ns</nuxt-link>
        </div>
        <ul class="sidebar-menu">
          <li class="menu-header">Dashboard</li>
          <li class="dropdown" :class="menu('dashboard')">
            <a href="javascript:void(0)" class="nav-link has-dropdown"
              ><i class="fas fa-fire"></i><span>Dashboard</span></a
            >
            <ul class="dropdown-menu">
              <li :class="menu('generalDashboard')">
                <nuxt-link class="nav-link" to="/dashboard/general"
                  >General Dashboard</nuxt-link
                >
              </li>
              <li :class="menu('ecommerceDashboard')">
                <nuxt-link class="nav-link" to="/dashboard/ecommerce"
                  >Ecommerce Dashboard</nuxt-link
                >
              </li>
            </ul>
          </li>
          <li class="menu-header">Starter</li>
          <li class="dropdown" :class="menu('layout')">
            <a
              href="javascript:void(0)"
              class="nav-link has-dropdown"
              data-toggle="dropdown"
              ><i class="fas fa-columns"></i> <span>Layout</span></a
            >
            <ul class="dropdown-menu">
              <li :class="menu('defaultLayout')">
                <nuxt-link class="nav-link" to="/starter/layout/defaultLayout"
                  >Default Layout</nuxt-link
                >
              </li>
            </ul>
          </li>
          <li :class="menu('blankPage')">
            <nuxt-link class="nav-link" to="/starter/blankPage"
              ><i class="far fa-square"></i> <span>Blank Page</span></nuxt-link
            >
          </li>
          <li class="dropdown" :class="menu('bootstrap')">
            <a href="javascript:void(0)" class="nav-link has-dropdown"
              ><i class="fas fa-th"></i> <span>Bootstrap</span></a
            >
            <ul class="dropdown-menu">
              <li :class="menu('alert')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/alert"
                  >Alert</nuxt-link
                >
              </li>
              <li :class="menu('badge')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/badge"
                  >Badge</nuxt-link
                >
              </li>
              <li :class="menu('breadcrumb')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/breadcrumb"
                  >Breadcrumb</nuxt-link
                >
              </li>
              <li :class="menu('buttons')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/buttons"
                  >Buttons</nuxt-link
                >
              </li>
              <li :class="menu('card')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/card"
                  >Card</nuxt-link
                >
              </li>
              <li :class="menu('carousel')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/carousel"
                  >Carousel</nuxt-link
                >
              </li>
              <li :class="menu('collapse')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/collapse"
                  >Collapse</nuxt-link
                >
              </li>
              <li :class="menu('dropdown')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/dropdown"
                  >Dropdown</nuxt-link
                >
              </li>
              <li :class="menu('form')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/form"
                  >Form</nuxt-link
                >
              </li>
              <li :class="menu('listGroup')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/listGroup"
                  >List Group</nuxt-link
                >
              </li>
              <li :class="menu('mediaObject')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/mediaObject"
                  >Media Object</nuxt-link
                >
              </li>
              <li :class="menu('modal')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/modal"
                  >Modal</nuxt-link
                >
              </li>
              <li :class="menu('nav')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/nav"
                  >Nav</nuxt-link
                >
              </li>
              <li :class="menu('navbar')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/navbar"
                  >Navbar</nuxt-link
                >
              </li>
              <li :class="menu('pagination')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/pagination"
                  >Pagination</nuxt-link
                >
              </li>
              <li :class="menu('popover')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/popover"
                  >Popover</nuxt-link
                >
              </li>
              <li :class="menu('progress')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/progress"
                  >Progress</nuxt-link
                >
              </li>
              <li :class="menu('table')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/table"
                  >Table</nuxt-link
                >
              </li>
              <li :class="menu('tooltip')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/tooltip"
                  >Tooltip</nuxt-link
                >
              </li>
              <li :class="menu('typography')">
                <nuxt-link class="nav-link" to="/starter/bootstrap/typography"
                  >Typography</nuxt-link
                >
              </li>
            </ul>
          </li>
          <li class="menu-header">Stisla</li>
          <li class="dropdown" :class="menu('components')">
            <a href="javascript:void(0)" class="nav-link has-dropdown"
              ><i class="fas fa-th-large"></i> <span>Components</span></a
            >
            <ul class="dropdown-menu">
              <li :class="menu('article')">
                <nuxt-link class="nav-link" to="/stisla/components/article"
                  >Article</nuxt-link
                >
              </li>
              <li :class="menu('avatar')">
                <nuxt-link
                  class="nav-link beep beep-sidebar"
                  to="/stisla/components/avatar"
                  >Avatar</nuxt-link
                >
              </li>
              <li :class="menu('chatBox')">
                <nuxt-link class="nav-link" to="/stisla/components/chatBox"
                  >Chat Box</nuxt-link
                >
              </li>
              <li :class="menu('emptyState')">
                <nuxt-link
                  class="nav-link beep beep-sidebar"
                  to="/stisla/components/emptyState"
                  >Empty State</nuxt-link
                >
              </li>
              <li :class="menu('gallery')">
                <nuxt-link class="nav-link" to="/stisla/components/gallery"
                  >Gallery</nuxt-link
                >
              </li>
              <li :class="menu('hero')">
                <nuxt-link
                  class="nav-link beep beep-sidebar"
                  to="/stisla/components/hero"
                  >Hero</nuxt-link
                >
              </li>
              <li :class="menu('multipleUpload')">
                <nuxt-link
                  class="nav-link"
                  to="/stisla/components/multipleUpload"
                  >Multiple Upload</nuxt-link
                >
              </li>
              <li :class="menu('pricing')">
                <nuxt-link
                  class="nav-link beep beep-sidebar"
                  to="/stisla/components/pricing"
                  >Pricing</nuxt-link
                >
              </li>
              <li :class="menu('tab')">
                <nuxt-link class="nav-link" to="/stisla/components/tab"
                  >Tab</nuxt-link
                >
              </li>
              <li :class="menu('table')">
                <nuxt-link class="nav-link" to="/stisla/components/table"
                  >Table</nuxt-link
                >
              </li>
              <li :class="menu('user')">
                <nuxt-link class="nav-link" to="/stisla/components/user"
                  >User</nuxt-link
                >
              </li>
              <li :class="menu('wizard')">
                <nuxt-link
                  class="nav-link beep beep-sidebar"
                  to="/stisla/components/wizard"
                  >Wizard</nuxt-link
                >
              </li>
            </ul>
          </li>
          <li class="dropdown" :class="menu('forms')">
            <a href="javascript:void(0)" class="nav-link has-dropdown"
              ><i class="far fa-file-alt"></i> <span>Forms</span></a
            >
            <ul class="dropdown-menu">
              <li :class="menu('advancedForm')">
                <nuxt-link class="nav-link" to="/stisla/forms/advancedForm"
                  >Advanced Form</nuxt-link
                >
              </li>
              <li :class="menu('editor')">
                <nuxt-link class="nav-link" to="/stisla/forms/editor"
                  >Editor</nuxt-link
                >
              </li>
              <li :class="menu('validation')">
                <nuxt-link class="nav-link" to="/stisla/forms/validation"
                  >Validation</nuxt-link
                >
              </li>
            </ul>
          </li>
        </ul>
      </aside>
    </div>
  </div>
</template>

<script>
import { mapState } from "vuex";
export default {
  computed: {
    ...mapState({ pages: (state) => state.pages }),
  },
  methods: {
    menu(menuName) {
      const name = menuName,
        current_page = this.pages.current_page;

      const split_current_page = current_page.split("-");
      if (split_current_page.length > 0) {
        if (name == split_current_page[0]) {
          return "active";
        }
        if (name == split_current_page[1]) {
          return "active";
        }
      } else {
        if (name == current_page) {
          return "active";
        }
        return "";
      }
    },
  },
};
</script>