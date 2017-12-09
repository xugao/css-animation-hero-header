# css-animation-hero-header
following steps from tutorial https://courses.cssanimation.rocks/

### Summary
```sass
header:before {
	animation: fade-slide-down 2s .1s cubic-bezier(0, .5, 0, 1) forwards;
	opacity: 0;
	background: linear-gradient(to bottom, rgba(0,0,0,0), rgba(0,0,0,.8)),
		url("../images/background.jpg") no-repeat bottom;

	background: cover;

	content: "";
	position: absolute;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
	z-index: -1;
}

@keyframes fade-slide-down {
	0% {
		opacity: 0;
		transform: translateY(-4rem);
	}
	100% {
		opacity: 1;
		transform: none;
	}
}
```

Getting free images here - https://unsplash.com

Create timing function - http://cubic-bezier.com/
