<template>
<div class="main-page-page page6" id="page6">
    <div class="content">
        <div class="title"><span class="my">나만의 것</span>을 만드는 <br>크리에이터가 되고 싶나요?</div>
        <div class="apply-warp" @click="applyClick">지금 지원하기</div>
    </div>
</div>
</template>

<script>
export default {
    name : "Page6",
    methods : {
        applyClick(e) {
            e
            open("https://form.edcan.kr")
        }
    }
}
</script>

<style scoped>
.page6, .content, .main-page-page{
    min-height: 0px;
}

.main-page-page {
    padding: 150px 0;
}

.content > * {
    display: inline-block;
    font-size: 48px;
    font-weight: bold;

    margin: 0 32px;
}

.title {
    color: #425563;
}

.title:hover .my {
    color: #00A9CE;
    transition: 250ms;
}

.apply-warp {
    color: #768692;

    cursor: pointer;

    transition: 250ms;
}

.apply-warp:hover {
    color: #00A9CE;
    transform: scale(1.015);
}

@media (max-width: 900px) {
    .content > * {
        font-size: 32px;
    }
}

@media (max-width: 500px) {
    .title {
        font-size: 27px;
    }

    .apply-warp {
        font-size: 31px;
    }
}
</style>