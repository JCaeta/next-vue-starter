<template>
    <div>
      <!-- Your component's HTML goes here -->
      <h1>ComponentRequest component</h1>
      <p>Put your HTML elements here</p>
      <button @click="getData">Get Data</button>
    </div>
  </template>
  
  <script>
  import {sendGetRequest} from '../../pages/api/HttpRequests';
  
  export default {
    name: 'ComponentRequest',
    data() {
      return {
        responseData: null
      }
    },
    methods: {
      async getData() {
        const response = await sendGetRequest();
        this.responseData = response.data;
        console.log(response.data);
      }
    }
  }
  </script>
  
  <style>
  /* Your component's CSS goes here */
  </style>