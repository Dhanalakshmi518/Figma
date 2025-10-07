# Ex09 Event Registration Web Application
## Date:7-10-2025

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
import React from "react";
import rectangle1 from "./rectangle-1.svg";

export const AndroidMedium = (): JSX.Element => {
  return (
    <main className="bg-[#fc1351] overflow-hidden w-full min-w-[3620px] min-h-[5530px] relative">
      <img
        className="absolute top-[5416px] left-[3684px] w-[993px] h-[292px]"
        alt="Rectangle"
        src={rectangle1}
      />

      <section
        className="absolute top-[2222px] left-[847px] w-[1620px] h-[543px] bg-[#fbeded]"
        aria-label="Register section"
      >
        <p className="absolute top-[149px] left-[167px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-xs tracking-[0] leading-[normal]">
          <span className="[font-family:'Inter-Regular',Helvetica] font-normal text-black text-xs tracking-[0]">
            RE&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;GIS
          </span>
          <span className="text-9xl">REGISTER</span>
        </p>
      </section>

      <section
        className="absolute top-[1594px] left-[862px] w-[1605px] h-[530px] bg-[#d9d9d9]"
        aria-label="Login section"
      >
        <div className="absolute top-[80px] left-[5px] w-[1600px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-9xl tracking-[0] leading-[normal]">
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{" "}
          <br />
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
          LOGIN
        </div>
      </section>
    </main>
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
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

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
import React from "react";
import screenshot202510071514051 from "./screenshot-2025-10-07-151405-1.png";

export const AndroidMedium = (): JSX.Element => {
  const eventActivities = [
    "DANCE",
    "SONG",
    "DJ",
    "RANGOLI",
    "FUN ACTIVITIES",
    "FIRELESS COOKING",
  ];

  return (
    <div className="bg-[#18e3fa] w-full min-w-[3363px] min-h-[5530px] relative">
      <img
        className="absolute top-0 left-0 w-[3363px] h-[5530px] aspect-[0.61] object-cover"
        alt="Cultural Event Poster"
        src={screenshot202510071514051}
      />

      <div className="absolute top-[1634px] left-[728px] w-[1666px]">
        <h1 className="[font-family:'Inter-Regular',Helvetica] font-normal text-black text-9xl tracking-[0] leading-[normal] mb-[144px] text-center">
          CULTURAL EVENT
        </h1>

        <ul
          className="[font-family:'Inter-Regular',Helvetica] font-normal text-black text-9xl tracking-[0] leading-[normal]"
          role="list"
        >
          {eventActivities.map((activity, index) => (
            <li key={index} className="mb-[72px] text-center">
              {activity}
            </li>
          ))}
        </ul>
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
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

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
import React, { useState } from "react";
import screenshot202510071525401 from "./screenshot-2025-10-07-152540-1.png";

export const AndroidMedium = (): JSX.Element => {
  const [formData, setFormData] = useState({
    name: "",
    registerNumber: "",
    department: "",
    mobileNumber: "",
    interestedEvent: "",
  });

  const formFields = [
    { label: "NAME:", name: "name", type: "text" },
    { label: "REGISTER NUMBER:", name: "registerNumber", type: "text" },
    { label: "DEPARTMENT:", name: "department", type: "text" },
    { label: "MOBILE NUMBER:", name: "mobileNumber", type: "tel" },
    { label: "INTERESTED EVENT:", name: "interestedEvent", type: "text" },
  ];

  const handleInputChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    const { name, value } = e.target;
    setFormData((prev) => ({
      ...prev,
      [name]: value,
    }));
  };

  return (
    <div className="bg-[#15fdfd] w-full min-w-[3105px] min-h-[5383px] relative">
      <header className="absolute top-[527px] left-[233px] w-[2486px] h-[657px] bg-[#d9d9d9]">
        <h1 className="absolute top-[251px] left-[413px] [font-family:'Inter-Regular',Helvetica] font-normal text-black text-9xl tracking-[0] leading-[normal]">
          EVENT DAY REGISTRATION
        </h1>
      </header>

      <main className="absolute top-[1358px] left-[619px] w-[1387px]">
        <form className="[font-family:'Inter-Regular',Helvetica] font-normal text-black text-9xl tracking-[0] leading-[normal]">
          {formFields.map((field, index) => (
            <div key={field.name} className={index > 0 ? "mt-[72px]" : ""}>
              <label htmlFor={field.name} className="block mb-4">
                {field.label}
              </label>
              <input
                type={field.type}
                id={field.name}
                name={field.name}
                value={formData[field.name as keyof typeof formData]}
                onChange={handleInputChange}
                className="w-full bg-transparent border-b-4 border-black px-2 py-4 [font-family:'Inter-Regular',Helvetica] font-normal text-black text-9xl tracking-[0] leading-[normal] focus:outline-none focus:border-[#0d9d9d]"
                aria-label={field.label}
              />
            </div>
          ))}
        </form>
      </main>

      <footer className="absolute top-[3042px] left-[130px] w-[2699px]">
        <address className="[font-family:'Inter-Regular',Helvetica] font-normal text-black text-9xl tracking-[0] leading-[normal] not-italic">
          FOR FURTHER DETAILS CONTACT ADMIN -<br />
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ARYA
          KRISHNA E<br />
          CONTACT NUMBER:123456789
        </address>
      </footer>

      <img
        className="absolute top-[4258px] left-[178px] w-[2604px] h-[769px] aspect-[3.39] object-cover"
        alt="Thank you message with colorful balloons and stars decoration"
        src={screenshot202510071525401}
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
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

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
![alt text](<Screenshot 2025-10-07 160400.png>)


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
