<template>
    <header class="flex items-center">
            <div style="height: 54px" class="pr-5">
              <img src="/logo.svg" alt="logo" class="h-full" />
            </div>
            <ul class="flex items-center">
              <li>
                <a
                  class="text-white hover:text-teal-500 text-lg px-4 py-3"
                  href="/"
                  >Home</a
                >
              </li>
              <li>
                <a
                  class="text-white hover:text-teal-500 text-lg px-4 py-3"
                  href="/projects.html"
                  >Project</a
                >
              </li>
              <li>
                <a
                  class="text-white hover:text-teal-500 text-lg px-4 py-3"
                  href="/features.html"
                  >Features</a
                >
              </li>
              <li>
                <a
                  class="text-white hover:text-teal-500 text-lg px-4 py-3"
                  href="/story.html"
                  >Success Stories</a
                >
              </li>
            </ul>
            <ul class="flex ml-auto items-center mt-2">
              <li>
                <nuxt-link to="/login" class="inline-block bg-transparent border-white border hover:bg-white hover:bg-opacity-25 text-white font-light w-40 text-center px-6 py-1 text-lg rounded-full mr-4"
                > Sign Up </nuxt-link>
              </li>
              <li>
                <a
                  href="/login.html"
                  class="inline-block bg-transparent border-white border hover:bg-white hover:bg-opacity-25 text-white font-light w-40 text-center px-6 py-1 text-lg rounded-full"
                >
                  My Account
                </a>
              </li>
            </ul>
          </header>
</template>

  
<style lang="scss">
    .header__bg {
      position: absolute;
      top: 0;
      bottom: 0;
      right: 0;
      left: 0;
      width: 100%;
      height: 640px;
      background-image: url('/auth-background.svg');
      background-position: top right;
      background-repeat: no-repeat;
      background-color: #3b41e3;
      transform: skewY(-6deg);
      transform-origin: top left;
    }
    
    .cta-clip {
      position: relative;
      top: 200px;
      bottom: 0;
      right: 0;
      left: 0;
      width: 100%;
      height: 300px;
      background-position: top right;
      background-size: 300px;
      background-repeat: no-repeat;
      background-color: #fff;
      transform: skewY(4deg);
      transform-origin: bottom right;
    }
    
    .call-to-action {
      background-image: url('/auth-background.svg');
      background-position: top right;
      background-repeat: no-repeat;
      background-size: 450px;
    }
    
    .card-project {
      transition: all 0.3s ease 0s, opacity 0.5s cubic-bezier(0.5, 0, 0, 1) 1ms;
      max-height: 485px;
      overflow: hidden;
    
      .button-cta {
        opacity: 0;
        transition: all 300ms ease;
      }
    
      &:hover {
        box-shadow: 0 4px 25px 0 rgba(0, 0, 0, 0.15);
    
        .button-cta {
          opacity: 1;
          transition: all 300ms ease;
        }
    
        .progress-bar,
        .progress-info {
          opacity: 0;
          height: 0px;
          margin: 0px;
          padding: 0px;
          transition: all 300ms ease;
        }
      }
    }
    
    footer {
      z-index: inherit;
    }
    
    .hero-underline {
      text-decoration-color: #1abc9c;
    }
    
    .testimonial-user {
      opacity: 0.4;
      &.active {
        opacity: 1;
        border: 5px solid #fff;
        box-shadow: 0 0 0 1px #3b41e3;
      }
    }
    </style>