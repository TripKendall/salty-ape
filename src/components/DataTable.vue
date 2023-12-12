<template>
  <section class="data-table-live-tream" id="leader-board">
    <div class="container">
      <div class="data-table-live-table position-relative">
        <div class="table-responsive">

          <div class="data-table-title d-md-flex text-center align-items-center justify-content-between">
            <h4 class="mb-md-0">Salty Ape Leader Board</h4>
            <a class="fs-5 text-decoration-underline" href="/#what">
              What the hell is this?
            </a>
          </div>

          <table class="table table-striped text-nowrap text-center text-lg-start">

            <thead>
              <tr>
                <th class="fs-5">#</th>
                <th class="fs-5">Name</th>
                <th class="fs-5">Rating</th>
                <th class="fs-5">Trend</th>
                <th class="fs-5">Status</th>
              </tr>
            </thead>

            <tbody>
              <tr v-for="link in data">

                <td class="fs-6"> {{ link.rank }} </td>

                <td class="fs-6">
                  <div class="coin-name d-flex align-items-center">
                    <div class="coin-img">
                      <img :src="link.img" :alt="link.name" class="leader-board-image">
                    </div>

                    <h6 class="coin-title mb-0">
                      <a :href="link.link" class="gray-link text-decoration-none">
                        {{ link.name }}
                      </a>
                      <span class="coin-title-small">
                        {{ link.symbol }}
                      </span>
                    </h6>

                  </div>
                </td>

                <td class="fs-6">{{ link.price }}</td>

                <td :class="{
                  'green-text': link.change.startsWith('+'),
                  'red-text': link.change.startsWith('-')
                }" class="fs-6">
                  {{ link.change }}
                </td>

                <td :class="{
                  'green-text': link.action === 'Buy',
                  'red-text': link.action !== 'Buy'
                }" class="fs-6">
                  {{ link.action }}
                </td>

              </tr>

            </tbody>
          </table>

        </div>
      </div>
    </div>

  </section>
</template>

<script setup>
import { data } from '../js/leaderBoardData.js'
</script>

<style scoped>
.leader-board-image {
  width: 33px !important;
  height: 33px !important;
  margin-right: 10px;
  border-radius: 999px;
}

.gray-link {
  color: #323342 !important;
}

.gray-link:hover {
  color: #5b0389 !important;
}
</style>