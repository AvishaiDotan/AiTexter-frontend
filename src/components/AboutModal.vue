<template>
  <div>
    <button @click="$emit('toggleAbout')" class="close-about-modal">
      <svg class="close-about-modal svg" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg" aria-hidden="true"
        role="presentation" focusable="false" style="
                    display: block;
                    fill: none;
                    height: 16px;
                    width: 16px;
                    stroke: currentcolor;
                    stroke-width: 3;
                    overflow: visible;
                  ">
        <path d="m6 6 20 20"></path>
        <path d="m26 6-20 20"></path>
      </svg>
    </button>
    <div class="about-intro">
      <h2>This OpenAI tool allows you to re-style any text you want</h2>
      <p>
        The converter uses a node.js server to deliver the request prompt to
        OpenAI servers, it can be easily modified to perform any task ChatGpt is
        capable of.
      </p>
    </div>
    <div class="about-info">
      <h4>To create it we used</h4>
      <ul>
        <li>
          Vue with composition API
          <svg viewBox="0 0 24 24" style="height: 20px; width: 20px; display: inline-block;">
            <path fill="currentColor"
              d="M2,3H5.5L12,15L18.5,3H22L12,21L2,3M6.5,3H9.5L12,7.58L14.5,3H17.5L12,13.08L6.5,3Z"></path>
          </svg>
        </li>
        <li>
          TypeScript
          <svg viewBox="0 0 24 24" style="height: 20px; width: 20px; display: inline-block;">
            <path fill="currentColor"
              d="M3,3H21V21H3V3M13.71,17.86C14.21,18.84 15.22,19.59 16.8,19.59C18.4,19.59 19.6,18.76 19.6,17.23C19.6,15.82 18.79,15.19 17.35,14.57L16.93,14.39C16.2,14.08 15.89,13.87 15.89,13.37C15.89,12.96 16.2,12.64 16.7,12.64C17.18,12.64 17.5,12.85 17.79,13.37L19.1,12.5C18.55,11.54 17.77,11.17 16.7,11.17C15.19,11.17 14.22,12.13 14.22,13.4C14.22,14.78 15.03,15.43 16.25,15.95L16.67,16.13C17.45,16.47 17.91,16.68 17.91,17.26C17.91,17.74 17.46,18.09 16.76,18.09C15.93,18.09 15.45,17.66 15.09,17.06L13.71,17.86M13,11.25H8V12.75H9.5V20H11.25V12.75H13V11.25Z">
            </path>
          </svg>
        </li>
        <li>
          Sass
          <svg viewBox="0 0 24 24" style="height: 20px; width: 20px; display: inline-block;">
            <path fill="currentColor"
              d="M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M10,15.33C10.16,15.87 10.14,16.37 10,16.83C10,16.88 9.96,16.93 9.94,17C9.92,17 9.9,17.07 9.87,17.12C9.76,17.36 9.6,17.59 9.41,17.79C8.83,18.43 8,18.67 7.67,18.47C7.29,18.25 7.5,17.35 8.16,16.64C8.88,15.88 9.92,15.38 9.92,15.38V15.38L10,15.33M18.27,6.28C17.82,4.5 14.87,3.92 12.09,4.91C10.43,5.5 8.63,6.42 7.34,7.63C5.81,9.07 5.56,10.32 5.66,10.84C6,12.68 8.54,13.89 9.58,14.78V14.79C9.28,14.94 7.04,16.07 6.5,17.23C5.96,18.45 6.6,19.33 7,19.45C8.34,19.81 9.69,19.16 10.41,18.07C11.11,17.03 11.06,15.68 10.75,15C11.17,14.9 11.66,14.85 12.28,14.92C14.04,15.13 14.38,16.22 14.31,16.68C14.25,17.14 13.88,17.39 13.76,17.47C13.64,17.54 13.6,17.57 13.61,17.63C13.62,17.71 13.68,17.71 13.78,17.69C13.93,17.66 14.71,17.32 14.74,16.47C14.78,15.39 13.75,14.19 11.93,14.22C11.18,14.24 10.71,14.31 10.37,14.44L10.29,14.35C9.16,13.15 7.08,12.3 7.17,10.68C7.2,10.09 7.4,8.55 11.17,6.67C14.25,5.13 16.72,5.55 17.15,6.5C17.76,7.83 15.83,10.32 12.63,10.68C11.41,10.82 10.76,10.34 10.6,10.17C10.43,10 10.41,9.97 10.35,10C10.24,10.07 10.31,10.23 10.35,10.33C10.44,10.58 10.84,11 11.5,11.24C12.09,11.43 13.53,11.54 15.26,10.87C17.2,10.12 18.72,8.03 18.27,6.28Z">
            </path>
          </svg>
        </li>
        <li>
          Node.js
          <svg viewBox="0 0 24 24" style="height: 20px; width: 20px; display: inline-block;">
            <path fill="currentColor"
              d="M12,1.85C11.73,1.85 11.45,1.92 11.22,2.05L3.78,6.35C3.3,6.63 3,7.15 3,7.71V16.29C3,16.85 3.3,17.37 3.78,17.65L5.73,18.77C6.68,19.23 7,19.24 7.44,19.24C8.84,19.24 9.65,18.39 9.65,16.91V8.44C9.65,8.32 9.55,8.22 9.43,8.22H8.5C8.37,8.22 8.27,8.32 8.27,8.44V16.91C8.27,17.57 7.59,18.22 6.5,17.67L4.45,16.5C4.38,16.45 4.34,16.37 4.34,16.29V7.71C4.34,7.62 4.38,7.54 4.45,7.5L11.89,3.21C11.95,3.17 12.05,3.17 12.11,3.21L19.55,7.5C19.62,7.54 19.66,7.62 19.66,7.71V16.29C19.66,16.37 19.62,16.45 19.55,16.5L12.11,20.79C12.05,20.83 11.95,20.83 11.88,20.79L10,19.65C9.92,19.62 9.84,19.61 9.79,19.64C9.26,19.94 9.16,20 8.67,20.15C8.55,20.19 8.36,20.26 8.74,20.47L11.22,21.94C11.46,22.08 11.72,22.15 12,22.15C12.28,22.15 12.54,22.08 12.78,21.94L20.22,17.65C20.7,17.37 21,16.85 21,16.29V7.71C21,7.15 20.7,6.63 20.22,6.35L12.78,2.05C12.55,1.92 12.28,1.85 12,1.85M14,8C11.88,8 10.61,8.89 10.61,10.39C10.61,12 11.87,12.47 13.91,12.67C16.34,12.91 16.53,13.27 16.53,13.75C16.53,14.58 15.86,14.93 14.3,14.93C12.32,14.93 11.9,14.44 11.75,13.46C11.73,13.36 11.64,13.28 11.53,13.28H10.57C10.45,13.28 10.36,13.37 10.36,13.5C10.36,14.74 11.04,16.24 14.3,16.24C16.65,16.24 18,15.31 18,13.69C18,12.08 16.92,11.66 14.63,11.35C12.32,11.05 12.09,10.89 12.09,10.35C12.09,9.9 12.29,9.3 14,9.3C15.5,9.3 16.09,9.63 16.32,10.66C16.34,10.76 16.43,10.83 16.53,10.83H17.5C17.55,10.83 17.61,10.81 17.65,10.76C17.69,10.72 17.72,10.66 17.7,10.6C17.56,8.82 16.38,8 14,8Z">
            </path>
          </svg>
        </li>
        <li>
          Git
          <svg viewBox="0 0 24 24" style="height: 20px; width: 20px; display: inline-block;">
            <path fill="currentColor"
              d="M2.6,10.59L8.38,4.8L10.07,6.5C9.83,7.35 10.22,8.28 11,8.73V14.27C10.4,14.61 10,15.26 10,16A2,2 0 0,0 12,18A2,2 0 0,0 14,16C14,15.26 13.6,14.61 13,14.27V9.41L15.07,11.5C15,11.65 15,11.82 15,12A2,2 0 0,0 17,14A2,2 0 0,0 19,12A2,2 0 0,0 17,10C16.82,10 16.65,10 16.5,10.07L13.93,7.5C14.19,6.57 13.71,5.55 12.78,5.16C12.35,5 11.9,4.96 11.5,5.07L9.8,3.38L10.59,2.6C11.37,1.81 12.63,1.81 13.41,2.6L21.4,10.59C22.19,11.37 22.19,12.63 21.4,13.41L13.41,21.4C12.63,22.19 11.37,22.19 10.59,21.4L2.6,13.41C1.81,12.63 1.81,11.37 2.6,10.59Z">
            </path>
          </svg>
        </li>
      </ul>
    </div>
    <div class="about-us">
      <div class="about-us img-container flex space-even">
        <a href="https://github.com/AvishaiDotan">
          
          <img  src="../../src/assets/avishai.jfif" alt="avatar" />
        </a>
        <a href="https://github.com/Nirosss">
          
          <img  src="../../src/assets/nir.jpg" alt="avatar" />
        </a>
        
      </div>
      <div class="about-us txt-container">
        <h5>Created by Nir Roiter & Avishai Dotan</h5>
      </div>
  </div>
</div></template>
