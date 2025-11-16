# Ex09 Event Registration Web Application
## Date:16/11/25

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
Home Page
import React from "react";
import image1 from "./image-1.png";
import image202511161757398011 from "./image-2025-11-16-175739801-1.png";
import rectangle2 from "./rectangle-2.png";

export const AndroidCompact = () => {
  return (
    <div className="bg-[#6100bd] w-full min-w-[360px] min-h-[640px] relative">
      <img
        className="absolute top-0 left-0 w-[360px] h-[132px] aspect-[3.28] object-cover"
        alt="Image"
        src={image202511161757398011}
      />

      <img
        className="absolute top-[132px] left-0 w-[360px] h-[299px] aspect-[1.28] object-cover"
        alt="Image"
        src={image1}
      />

      <div className="absolute top-[174px] left-[111px] w-[138px] [font-family:'Inter-Black',Helvetica] font-black text-black text-xl text-center tracking-[0] leading-[normal] whitespace-nowrap">
        SPORTS DAY EVENT
      </div>

      <div className="absolute top-[457px] left-[88px] w-[184px] h-8 bg-black rounded-[20px] border border-solid border-white shadow-[0px_4px_4px_#00000040]" />

      <img
        className="absolute top-[515px] left-[84px] w-48 h-10"
        alt="Rectangle"
        src={rectangle2}
      />

      <div className="absolute top-[523px] left-[148px] [font-family:'Inter-Black',Helvetica] font-black text-white text-xl text-center tracking-[0] leading-[normal]">
        LOGIN
      </div>

      <div className="absolute top-[465px] left-[130px] [font-family:'Inter-Black',Helvetica] font-black text-white text-xl text-center tracking-[0] leading-[normal]">
        REGISTER
      </div>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

The Events
import React from "react";
import image2 from "./image-2.png";
import line1 from "./line-1.png";

export const IphoneProMax = () => {
  return (
    <div className="bg-[#5b1414] w-full min-w-[360px] min-h-[640px] relative">
      <img
        className="absolute top-0 left-0 w-[360px] h-[640px] aspect-[1] object-cover"
        alt="Image"
        src={image2}
      />

      <div className="absolute top-[90px] left-[91px] [font-family:'Inter-Black',Helvetica] font-black text-black text-3xl text-center tracking-[0] leading-[normal]">
        The Events:
      </div>

      <div className="absolute top-[162px] left-[71px] [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal]">
        Badminton
        <br />
        Javelin Throw
        <br />
        Water Polo
        <br />
        Fencing
        <br />
        Squash
        <br />
        Archery
        <br />
        Rugby
        <br />
        Figure Skating
        <br />
        Handball
        <br />
        Surfing
      </div>

      <img
        className="absolute top-[129px] left-[calc(50.00%_-_99px)] w-[197px] h-[15px]"
        alt="Line"
        src={line1}
      />
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

Registration details:
import React from "react";
import image2 from "./image-2.png";
import line1 from "./line-1.png";

export const IphoneProMax = () => {
  return (
    <div className="bg-[#5b1414] overflow-hidden w-full min-w-[360px] min-h-[640px] relative">
      <img
        className="absolute top-0 left-0 w-[360px] h-[640px] aspect-[1] object-cover"
        alt="Image"
        src={image2}
      />

      <div className="top-[218px] left-4 bg-black rounded-[20px] absolute w-56 h-[33px] border border-solid shadow-[0px_4px_4px_#00000040]" />

      <div className="absolute top-[27px] left-3 [font-family:'Inter-Black',Helvetica] font-black text-black text-3xl text-center tracking-[0] leading-[normal] whitespace-nowrap">
        Registration Form:
      </div>

      <div className="absolute top-28 left-4 [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal]">
        Fill in the Details:
      </div>

      <img
        className="absolute top-[68px] left-[calc(50.00%_-_172px)] w-[301px] h-[15px]"
        alt="Line"
        src={line1}
      />

      <div className="top-[167px] left-4 bg-black rounded-[20px] absolute w-56 h-[33px] border border-solid shadow-[0px_4px_4px_#00000040]" />

      <div className="top-[318px] left-4 bg-black rounded-[20px] absolute w-56 h-[33px] border border-solid shadow-[0px_4px_4px_#00000040]" />

      <div className="top-[269px] left-4 bg-black rounded-[20px] absolute w-56 h-[33px] border border-solid shadow-[0px_4px_4px_#00000040]" />

      <div className="top-[419px] left-4 bg-black rounded-[20px] absolute w-56 h-[33px] border border-solid shadow-[0px_4px_4px_#00000040]" />

      <div className="top-[368px] left-4 bg-black rounded-[20px] absolute w-56 h-[33px] border border-solid shadow-[0px_4px_4px_#00000040]" />

      <div className="top-[521px] left-4 bg-black rounded-[20px] absolute w-56 h-[33px] border border-solid shadow-[0px_4px_4px_#00000040]" />

      <div className="top-[470px] left-4 bg-black rounded-[20px] absolute w-56 h-[33px] border border-solid shadow-[0px_4px_4px_#00000040]" />

      <div className="absolute top-[167px] left-[58px] [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal]">
        Full Name:
      </div>

      <div className="absolute top-[218px] left-[75px] [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal]">
        Gender:
      </div>

      <div className="absolute top-[266px] left-[100px] [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal] whitespace-nowrap">
        Age:
      </div>

      <div className="absolute top-[318px] left-[72px] [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal] whitespace-nowrap">
        Email Id:
      </div>

      <div className="absolute top-[368px] left-16 [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal] whitespace-nowrap">
        Regd No.:
      </div>

      <div className="absolute top-[418px] left-10 [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal] whitespace-nowrap">
        Department:
      </div>

      <div className="absolute top-[470px] left-[55px] [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal] whitespace-nowrap">
        Mobile No:
      </div>

      <div className="absolute top-[521px] left-5 [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal] whitespace-nowrap">
        Events chosen:
      </div>

      <div className="top-[584px] left-20 bg-[#fe0000] border-black absolute w-56 h-[33px] border border-solid shadow-[0px_4px_4px_#00000040]" />

      <div className="absolute top-[584px] left-[132px] [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal]">
        SUBMIT
      </div>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

Thank You

import React from "react";
import image2 from "./image-2.png";
import image202511161757398011 from "./image-2025-11-16-175739801-1.png";

export const IphoneProMax = () => {
  return (
    <div className="bg-[#5b1414] w-full min-w-[360px] min-h-[640px] relative">
      <img
        className="absolute top-0 left-0 w-[360px] h-[640px] aspect-[1] object-cover"
        alt="Image"
        src={image2}
      />

      <div className="absolute top-[90px] left-[91px] [font-family:'Inter-Black',Helvetica] font-black text-black text-3xl text-center tracking-[0] leading-[normal]">
        The Events:
      </div>

      <img
        className="absolute top-0 left-0 w-[360px] h-[132px] aspect-[3.28] object-cover"
        alt="Image"
        src={image202511161757398011}
      />

      <div className="absolute top-[195px] left-3 [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal]">
        Thanks for registering
      </div>

      <div className="absolute top-[252px] left-[165px] w-[30px] [font-family:'Inter-Black',Helvetica] font-black text-white text-[100px] text-center tracking-[0] leading-[normal] whitespace-nowrap">
        😄
      </div>

      <div className="absolute top-[401px] left-0 [font-family:'Inter-Black',Helvetica] font-black text-white text-3xl text-center tracking-[0] leading-[normal]">
        Contact Info:
        <br />
        Email:sec@gmail.com
        <br />
        Phone No.:1234567890
      </div>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

```
## OUTPUT:

![alt text](image.png)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
