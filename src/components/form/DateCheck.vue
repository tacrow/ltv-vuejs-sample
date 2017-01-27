<template>
<div class="c-form-box">
  <h2 class="c-form-header">期間設定<span>（必須）</span></h2>
  <div class="p-date-form">
	<input type="button" class="c-btn" value="期間を追加">
	<input type="button" class="c-btn" value="期間をリセット">
  </div>
  <ul class="p-date-list">
  	<li class="p-date-list__item">
  	  <span>1：</span>
  	  <input type="date" class="c-input-date" value="2017-01-27">
  	  <span>&nbsp;〜&nbsp;</span>
  	  <input type="date" class="c-input-date" value="">
  	  <input type="button" class="c-btn" value="削除">
  	</li>
  	<li class="p-date-list__item">
  	  <span>2：</span>
  	  <input type="date" class="c-input-date" value="2017-01-27">
  	  <span>&nbsp;〜&nbsp;</span>
  	  <input type="date" class="c-input-date" value="">
  	  <input type="button" class="c-btn" value="削除">
  	</li>
  	<li class="p-date-list__item">
  	  <span>3：</span>
  	  <input type="date" class="c-input-date" value="2017-01-27">
  	  <span>&nbsp;〜&nbsp;</span>
  	  <input type="date" class="c-input-date" value="">
  	  <input type="button" class="c-btn" value="削除">
  	</li>
  </ul>
</div>
</template>

<style scoped>
.p-date-form {
	margin-bottom: 10px;
	padding-bottom: 10px;
}
.p-date-list {
  padding:  10px;
  border: 1px solid #a9a9a9;
  border-radius: 3px;
}
.p-date-list__item {
  position: relative;
  padding: 10px;
  margin-bottom: 10px;
  background-color: #ffffff;
  border: 1px solid #a9a9a9;
  border-radius: 3px;
  &:last-child {
  	margin-bottom: 0;
  }
  &:hover {
  	background-color: #eeeeee;
  }
  .c-btn {
  	position: absolute;
  	top: 50%;
  	right: 10px;
  	margin-top: -12px;
  }
}

</style>