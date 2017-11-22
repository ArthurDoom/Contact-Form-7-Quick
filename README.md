# Contact-Form-7-Quick
A quick copy and paste to layout the wordpress plugin Contact Form 7 

## The form

Example:

```html
<div class="contact-wrap clearfix">
<div class="contact-col-1">
	[text* your-name class:input-lg]First Name[/text*]
</div>
<div class="contact-col-2">
	[text* your-last-name class:input-lg]Last Name[/text*]
</div>
<div class="contact-col-1">
	[email* your-email class:input-lg]Email[/email*]
</div>
<div class="contact-col-2">
	[tel tel-num class:input-lg]Phone[/tel]
</div>
<div class="contact-col-full">
	[textarea* your-message]Your Message[/textarea*]
</div>
<div class="contact-col-full">
	[submit class:btn-block class:btn-lg]
</div>
</div><!--/-contact-wrap-->
```

## The Mail

Example:

```html

[your-name] [your-last-name]

email: [your-email]
tel: [tel-num]

[your-message]

This was sent from www.########.com

```

## Less 

Edit to suit:

```less 

.contact-wrap {
	padding: 30px;
	float: left;
	width: 100%;
	.border-box;
	.box-shadow;
	background-color: @white;
	@media (min-width: 992px) {
		padding: 60px;
	}

	label {
		color: #93939e;
	}
	.required {
		color: #ff4d5b;
	}
}

.contact-col-full,
.contact-col-1,
.contact-col-2 {
	float: left;
	width: 100%;
	padding: 0;
	.border-box;
	margin-top: 15px;
	@media (min-width: 992px) {
		margin-top: 25px;
	}
}

.contact-col-1 {
	@media (min-width: 992px) {
		width: 50%;
		padding-right: 10px;
	}
}
.contact-col-2 {
	@media (min-width: 992px) {
		width: 50%;
		padding-left: 10px;
	}
}

```
