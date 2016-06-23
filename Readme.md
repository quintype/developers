---
layout: page
title: Documentation
permalink: /docs/home
---
# Quintype for Developers

This repository is a knowledge base for developers working on projects backed by the Quintype platform.

### Basic Concepts

* The [Stories, Cards and Elements](./stories-cards-and-elements.md) has an explanation of the basic building blocks of a Quintype story.
* [Stacks](./stacks.md) are the easiest way to group stories together for various widgets on the page.
* [Story Collections](./story-collections.md) can be used for more advanced grouping, and for building of logical entities such as Magazine Issues or Courses.
* [Story Groups](./story-groups.md) is an important parameter which is passed to the stories API, determining the resulting stories.

### API Documentation

The [API Documentation](https://itsman.quintype.com/sketches-swagger.json) is available in [swagger](http://swagger.io) format. This can be pasted into the [Swagger Editor](http://editor.swagger.io/#/?import=https://itsman.quintype.com/sketches-swagger.json) to see a live view of the documentation.

### Preview

The [Preview](preview.md) section has information on getting preview to work.

### Image Sizes

The [Image](images.md) section has information on resizing images hosted by the Quintype platform.

### Sample Applications and Libraries

We have published a number of starter-kits for various popular languages. Please clone these, and use this as a starting point.

#### Front End Javascript

* The Image resizing functions is available via the [quintype-js](https://github.com/quintype/quintype-js) npm module

#### Ruby on Rails

The Ruby on Rails starter kit can be found here: [Coconut](https://github.com/quintype/coconut). The following libraries are used (and patches appreciated)

* [Quintype Ruby API](https://github.com/quintype/quintype-api-ruby)
* [Quintype Liquid](https://github.com/quintype/quintype-liquid)
* [Quintype Routes](https://github.com/quintype/quintype-routes)

#### PHP (with Laravel)

The PHP / Laravel application can be found here: [Pina Colada](https://github.com/quintype/pina-colada)
