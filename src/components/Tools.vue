<script setup>
import tools from '../data/tools.json';
</script>

<template>
	<!-- tools -->
    <div class="row flex-column bg-white jumbotron" id="tools">
        <h1 class="my-1 text-center" >Tools</h1>
        <div class="row justify-content-center py-3 tools-img">
            <div class="col-md-3 col-lg-2 mx-4 my-3">
                <h3 class="my-3 text-center">Front End</h3>
                <div class="row justify-content-center tools-img gx-5">
                    <div v-for="tool in tools.frontEnd" :key="tool.name" class="col-6 tools-img">
                        <img :src="tool.icon" :alt="tool.name" class="img-fluid">
                        <p class="tool-name mt-2">{{ tool.name }}</p>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-lg-2 mx-4 my-3">
                <h3 class="my-3 text-center">MERN</h3>
                <div class="row tools-img gx-5">
                    <div v-for="tool in tools.mern" :key="tool.name" class="col-6 tools-img">
                        <img :src="tool.icon" :alt="tool.name" class="img-fluid">
                        <p class="tool-name mt-2">{{ tool.name }}</p>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-lg-2 mx-4 my-3">
                <h3 class="my-3 text-center">Other Tools</h3>
                <div class="row tools-img gx-5">
                    <div v-for="tool in tools.other" :key="tool.name" class="col-6 tools-img">
                        <img :src="tool.icon" :alt="tool.name" class="img-fluid">
                        <p class="tool-name mt-2">{{ tool.name }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style>

</style>
