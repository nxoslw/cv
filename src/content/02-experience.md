## Experience

- ##### June 2020 – present

  ### Freelance

  #### Full-Stack Laravel Web Artisan

  - Crafting a **unified and consistent user experience** across web by creating and refining design patterns, components, and guidelines.
  - **Collaborating with cross-functional teams**, including designers, developers, and product managers, to ensure efficient and cohesive development processes.
  - Contributing to **enhancing the quality and usability**.
  - **Mentoring and guiding** fellow engineers, cultivating a culture of collaboration.

  > _LARAVEL_ _VueJS_ _NuxtJS_ _TailwindCSS_

- ##### March 2015 - May 2020

  ### BITSNACH

  #### Full-Stack Web Developer

  **BITSNACH** is a company with experience in creating and managing specialized online websites with global reach.

  - Created a scalable **Business website** running the company's online presence.
  - Improved sites **SEO** under the guidance of Google experts.
  - Coded a variety of tools for maintaining, extending, and **enhancing security**.

  > _PHP_ _MySQL_ _LARAVEL_ _VueJS_ _LESS_ _JavaScript_ _jQuery_ _Bootstrap_ _TailwindCSS_ _NodeJS_

- ##### 2014 – March 2015

  ### Freelance

  #### Frontend Developer

  > _HTML_ _CSS_ _Bootstrap_ _JavaScript_ _jQuery_

- ##### 15th November 1997

  ### Born

<style lang="scss">
  @import '../styles/theme.scss';

  :global(.wrapper) > ul {
    position: relative;

    &::before {
      background-color: lighten($background-color, 5%);
      bottom: 0;
      content: ' ';
      left: 20%;
      margin-left: -1px;
      position: absolute;
      top: 0;
      width: 2px;
    }

    > li {
      margin: 0 0 0 20%;
      max-width: 66em;
      padding-left: 2em;
      position: relative;
      width: 80%;

      + li {
        margin-top: 3em;
      }

      > h3 {
        line-height: 1.1;
      }

      > h5 {
        background: darken($heading-color, 2%);
        border-radius: 8px;
        padding: 2px 10px;
        position: absolute;
        right: 104%;
        text-shadow: 0 1px darken($heading-color, 30%);
        white-space: nowrap;
      }

      &::before {
        left: 0;
        margin: 0;
        position: absolute;
        transform: translateX(-50%);
      }
    }

    @media screen and (max-width: 1022px) {
      &::before {
        left: -1.2em;
      }

      > li {
        margin-left: 0;
        max-width: 100%;
        padding-left: 0.5em;
        width: 100%;

        > h5 {
          display: inline-block;
          margin-bottom: 1.2em;
          position: static;
          right: auto;
        }

        &::before {
          transform: translateX(-1.5em);
        }
      }
    }
  }
</style>
