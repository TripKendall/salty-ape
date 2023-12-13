<template>
  <section class="leader-board" id="leader-board">
    <div class="container">
      <div class="data-table-wrapper position-relative">
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
                <th>#</th>
                <th>Name</th>
                <th>Rating</th>
                <th>Trend</th>
                <th>Status</th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="link in data">
                <td> {{ link.rank }} </td>
                <td>
                  <div class="link-name d-flex align-items-center">
                    <div class="link-img">
                      <img :src="link.img" :alt="link.name" class="leader-board-image">
                    </div>
                    <h6 class="link-url mb-0">
                      <a :href="link.link" class="gray-link text-decoration-none">
                        {{ link.name }}
                      </a>
                      <span class="link-symbol">
                        {{ link.symbol }}
                      </span>
                    </h6>
                  </div>
                </td>
                <td>{{ link.rating }}</td>
                <td :class="{
                  'green-text': link.change.startsWith('+'),
                  'red-text': link.change.startsWith('-')}">
                  {{ link.change }}
                </td>
                <td :class="{
                  'green-text': link.action === 'Buy',
                  'red-text': link.action !== 'Buy'}">
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
