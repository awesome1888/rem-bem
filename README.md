# Rem-Bem

Rem-Bem is a LESS macros library that is useful for rem-based markups in the best traditions of BEM.

This package was basically tested only with Meteor (sorry, guys). It exports a set of `.less` files, so if you are a happy person with the meteor project at hand, check this package out!

## Installation

`meteor npm install rem-bem --save`

## Usage

Just do
~~~~
@import "{}/node_modules/rem-bem/less/index.less";
~~~~
somewhere inside your `/client/style/index.less` folder.

## The Concept

`@offset` is a basic metric unit, which equals to `1rem`

You can use mixins to include inside your LESS declaration, like the following:

~~~~
.my_button
{
    ._padding_x(2); // add padding equals to @offset * 2
    ._margin-b_x(0.5); // add margin bottom equals to @offset * 0.5
}
~~~~

Also, you can include the pre-existed classes directly inside the tag, as BEM taught us:
~~~~
<div class="padding_x2 margin-b_x0p5">Some useful information</div>
~~~~
These classes always go with `!important` instructions, so they cannot be overridden with other declarations. If you do not need the class anymore, you simply remove it from the tag, don't you?

## What do we have inside (reference)

Will finish when have time ;)

## License

MIT
