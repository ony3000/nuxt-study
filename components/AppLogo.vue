<template>
	<div class="VueToNuxtLogo">
		<div class="Triangle Triangle--two"/>
		<div class="Triangle Triangle--one"/>
		<div class="Triangle Triangle--three"/>
		<div class="Triangle Triangle--four"/>
	</div>
</template>

<style>
.VueToNuxtLogo {
	display: inline-block;
	animation: turn 2s linear forwards 1s;
	transform: rotateX(180deg);
	position: relative;
	overflow: hidden;
	height: 72px;
	width: 98px;
	vertical-align: bottom;
}

.Triangle {
	position: absolute;
	top: 0;
	left: 0;
	width: 0;
	height: 0;
}

.Triangle--one {
	border-left: 42px solid transparent;
	border-right: 42px solid transparent;
	border-bottom: 72px solid #41B883;
}

.Triangle--two {
	top: 12px;
	left: 14px;
	animation: goright 0.5s linear forwards 3.5s;
	border-left: 35px solid transparent;
	border-right: 35px solid transparent;
	border-bottom: 60px solid #3B8070;
}

.Triangle--three {
	top: 24px;
	left: 14px;
	animation: goright 0.5s linear forwards 3.5s;
	border-left: 28px solid transparent;
	border-right: 28px solid transparent;
	border-bottom: 48px solid #35495E;
}

.Triangle--four {
	top: 48px;
	left: 28px;
	animation: godown 0.5s linear forwards 3s;
	border-left: 14px solid transparent;
	border-right: 14px solid transparent;
	border-bottom: 24px solid #fff;
}

@keyframes turn {
	100% {
		transform: rotateX(0deg);
	}
}

@keyframes godown {
	100% {
		top: 72px;
	}
}

@keyframes goright {
	100% {
		left: 28px;
	}
}
</style>
