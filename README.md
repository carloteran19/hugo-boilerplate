# HUGO-Boilerplate

Out of the box site built with [HUGO](https://gohugo.io/) and [HUGO Pipes](https://gohugo.io/hugo-pipes/introduction/) as the asset pipeline.

This site uses [SASS](https://sass-lang.com/) as the CSS preprocessor.  SASS/SCSS files are compiled and minified by HUGO Pipes. 

SVG, CSS, and JS files are minified by [HUGO Pipes - Asset minification](https://gohugo.io/hugo-pipes/minification/)

TODO: Add Image compressor and optimizer. 

# Installation

## Prerequisites

You must have [HUGO](https://gohugo.io/getting-started/installing/) installed in your computer. 
>Make sure you are using v0.43 or higher. 

## Setup

Clone the repository to your local machine, cd to the project folder and run: 

    hugo server

# Development

## Responsive Web Design

This site follows the principles of [Responsive Web Design](https://alistapart.com/article/responsive-web-design) that consists on:

- Flexible grid-based layout. 
- Media Queries. 
- Images that resize. 

In order to ease collaboration and scalability this project uses the following **architecture**:

## 7-1 Pattern

> To get familiar with the 7-1 pattern read the [documentation](https://sass-guidelin.es/#architecture). 

### 7-1 Project structure
```
.
sass/
|
|– abstracts/
|   |– _variables.scss    # Sass Variables
|   |– _functions.scss    # Sass Functions
|   |– _mixins.scss       # Sass Mixins
|   |– _placeholders.scss # Sass Placeholders
|
|– base/
|   |– _reset.scss        # Reset/normalize
|   |– _typography.scss   # Typography rules
|   …                     # Etc.
|
|– components/
|   |– _buttons.scss      # Buttons
|   |– _carousel.scss     # Carousel
|   |– _cover.scss        # Cover
|   |– _dropdown.scss     # Dropdown
|   …                     # Etc.
|
|– layout/
|   |– _navigation.scss   # Navigation
|   |– _grid.scss         # Grid system
|   |– _header.scss       # Header
|   |– _footer.scss       # Footer
|   |– _sidebar.scss      # Sidebar
|   |– _forms.scss        # Forms
|   …                     # Etc.
|
|– pages/
|   |– _home.scss         # Home specific styles
|   |– _contact.scss      # Contact specific styles
|   …                     # Etc.
|
|– themes/
|   |– _theme.scss        # Default theme
|   |– _admin.scss        # Admin theme
|   …                     # Etc.
|
|– vendors/
|   |– _bootstrap.scss    # Bootstrap
|   |– _jquery-ui.scss    # jQuery UI
|   …                     # Etc.
|
`– main.scss              # Main Sass file
```

## BEM Architecture

> Read the [documentation](http://getbem.com/introduction/)  and this [guide](https://css-tricks.com/bem-101/) to learn more about BEM Architecture.


# Project Structure

```
.
 ├── archetypes/ // Contains Forestry.io configuration files
 ├── content/ // Where all site content is stored
 ├── data/ // TOML, YAML or JSON files containing site data
 ├── layouts/ // Your site's layouts
 ├── resources/ // Your site's partials
 ├── static/ // Where all static files live
 ├── themes/ // Where the default theme lives.
 | ├── boilerplate/ // default theme name, it can be changed based on project.
 | |   ├── boilerplate/ // default theme name, it can be changed based on project.
 | |   ├── boilerplate/ // default theme name, it can be changed based on project.
 └── config.toml // The Hugo configuration file
```
# Deployment

TODO: Deployment on Netlify. 