# Personal Portfolio Project

Welcome to my personal portfolio project, showcasing my journey as a junior software developer. This portfolio is built using HTML and SCSS (Sass).

## Table of Contents

1. [Project Overview](#project-overview)
2. [HTML Structure](#html-structure)
3. [SCSS Styles](#scss-styles)
4. [Media Queries](#media-queries)
5. [About me](#about-me)

## Project Overview

This portfolio serves as a platform to present my skills, projects, and contact information to potential employers and collaborators. It includes the following sections:

- **Header**: Contains my name and navigation links.
- **Summary**: A brief introduction with a headline.
- **About Me**: Details about myself and my passion for web development.
- **Technical Skills**: Icons representing my technical skills.
- **Projects**: A showcase of my projects, including project descriptions, images, and links.
- **Footer**: Links to my GitHub and LinkedIn profiles, as well as my email address.

## HTML Structure

The HTML structure is divided into sections, making it easy to navigate and understand the content. Each section corresponds to a part of the webpage, such as the header, about me, skills, and projects.

## SCSS Styles

### Responsive Design

- The project uses SCSS to create responsive designs. Media queries are employed to adapt the layout based on the screen size. For example, the "About Me" section changes from a column layout on smaller screens to a row layout on larger screens:

```scss
@media screen and (min-width: 1024px) {
  .aboutMe {
    /* Styles for larger screens */
  }
}
```

### CSS Grid and Flexbox

- CSS Grid and Flexbox are utilized to create grid layouts and align elements within sections. For instance, in the "Projects" section, Flexbox is used to arrange project cards in rows on smaller screens and columns on larger screens.

```scss
.project__holder {
  display: flex;
  flex-direction: column;

  @media screen and (min-width: 1024px) {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    /* Other grid styles */
  }
}
```

## Media Queries

- Media queries are used to make the webpage responsive, adjusting the layout and styling based on screen size. For instance, fonts, image sizes, and column/row layouts are modified for larger screens using media queries.

```scss
@media screen and (min-width: 1024px) {
  .projects {
    h2 {
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .project__holder {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      grid-template-rows: 1fr 1fr;

      .project__card {
        width: 25vw;
        height: auto;

        .project__image {
          margin: 5px;
          img {
            margin: 0px;
          }
        }
      }

      .project__button {
        display: flex;
        flex-direction: row;
      }

      .project__reactHeader {
        font-size: 1.25em;
      }

      .project__clientHeader {
        font-size: 1.6em;
      }
    }
  }
}
```

## About me

I'm a junior software developer currently based in Nottingham, UK, on a journey to become a full-stack developer. My passion for technology and web development drives me to constantly seek new challenges and expand my knowledge in the field. I'm dedicated to bringing my unique perspective to the world of software development by creating accessible and innovative solutions that address the practical needs of clients. Let's collaborate and build something remarkable together!
