<template>
  <b-container class="p-4 bg-dark border border-danger">
    <b-row class="p-2 bg-light d-flex justify-content-center border border-warning">
      <b-img src="https://einoo.files.wordpress.com/2012/03/wqt3y.gif" fluid class="border border-success"/>
    </b-row>
    <b-row class="p-2 bg-light">
      <b-col>
        <b-row class="d-flex justify-content-center">
          Page in maintenance
        </b-row>
      </b-col>
      <b-col>
        <b-row class="d-flex justify-content-center">
          <NuxtLink to="/home">
            Go to the older one!
          </NuxtLink>
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>