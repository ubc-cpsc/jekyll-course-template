# README

- [Intro](#intro)
- [Quickstart](#quickstart)
- [Adding to Your Course](#adding-to-your-course)

## Intro

This is a [Jekyll](https://jekyllrb.com/) template intended to be used as a starting point for creating a course website with the [UBC CLF Jekyll Theme](https://github.com/ubc-cpsc/jekyll-clf-theme) in the UBC CS webspace. You can see a working demo here: TO DO

## Quickstart

### Local Testing

Requirements: All the [Jekyll requirements](https://jekyllrb.com/docs/installation/#requirements)

```
git clone git@github.com:ubc-cpsc/jekyll-course-template.git # clone this repo
cd jekyll-course-template
bundle config set --local path 'vendor/bundle' #
bundle install # install the gems from the Gemfile
bundle jekyll exec serve # 
```

### Deployment

If you are wanting to host your website in the UBC Computer Science department webspace, please find the full deployment instructions on my.cs.

More on deploying Jekyll websites [here](https://jekyllrb.com/docs/deployment/). 

## Adding to Your Course

We use Jekyll [Collections](https://jekyllrb.com/docs/collections/) to make adding to the course simple.
There are 3 items you can add:
1) Lectures
2) Assignments
3) Tutorials

You can also always add your own custom pages in html, or markdown. For more information see the [Jekyll Docs](https://jekyllrb.com/docs/step-by-step/).

### Adding Lectures

Create a markdown file in the `_lectures` folder

Add:
- name
- description
- link

You can see [_lectures/lecture_1.md](_lectures/lecture_1.md?plain=1) as an example. Rebuild the site and the information will be added to the lectures page.

### Adding Assignments

Repeat the same steps with _assignments.

### Adding Tutorials

Repeat the same steps with _tutorials, plus add material outside of the front matter

This will also create a page at `/tutorials/<tutorial_name>.html`

You can see [_tutorials/tutorial-1.md](_tutorials/tutorial-1.md?plain=1) as an example.
