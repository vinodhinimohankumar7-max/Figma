# Ex08 Event Registration Web Application
## Date:19.12.2025

## AIM:
To design, develop and deploy a web application for event registration using Figma UI tool.

## UI DESIGN TOOL:
Figma

## DESIGN STEPS:

### Step 1:
Use frames to represent screens or sections.

### Step 2:
Add column grids for consistent spacing and alignment.

### Step 3:
Insert shapes, text, buttons, and icons.

### Step 4:
Use Auto Layout for flexible, responsive design.

### Step 5:
Define color, text, and effect styles globally for consistency.

### Step 6:
Name layers logically and group related elements.

### Step 6:
Link frames to show navigation or interactions.

### Step 7:
Select the specific frame while generating code using Anima plugin.

## CODE:
```
home page

import React from "react";
import onam1 from "./onam-1.png";
import seclogo11 from "./seclogo1-1.png";
import seclogo21 from "./seclogo2-1.png";

export const Frame = (): JSX.Element => {
  return (
    <div className="bg-white w-full min-w-[1568px] min-h-[2344px] relative">
      <img
        className="absolute top-[1565px] left-[471px] w-[564px] h-[564px] aspect-[1] object-cover"
        alt="Onam"
        src={onam1}
      />

      <div className="absolute top-[-778px] left-[1124px] w-[276px] h-[696px] rotate-[-0.99deg] bg-[linear-gradient(0deg,rgba(22,25,228,0.9)_0%,rgba(22,25,228,0.9)_100%),linear-gradient(0deg,rgba(217,217,217,1)_0%,rgba(217,217,217,1)_100%)]" />

      <img
        className="absolute top-0 left-0 w-[1564px] h-[302px] aspect-[5.37]"
        alt="Seclogo"
        src={seclogo11}
      />

      <img
        className="absolute top-[302px] left-[508px] w-[547px] h-[528px] aspect-[1.04]"
        alt="Seclogo"
        src={seclogo21}
      />

      <div className="absolute top-[891px] left-[93px] w-[1382px] h-[229px] bg-[linear-gradient(0deg,rgba(88,10,79,0.71)_0%,rgba(88,10,79,0.71)_100%),linear-gradient(0deg,rgba(167,195,28,0.69)_0%,rgba(167,195,28,0.69)_100%),linear-gradient(0deg,rgba(217,217,217,1)_0%,rgba(217,217,217,1)_100%)]" />

      <div className="absolute top-[1203px] left-[380px] w-[668px] h-[173px] bg-[linear-gradient(0deg,rgba(16,30,151,0.78)_0%,rgba(16,30,151,0.78)_100%),linear-gradient(0deg,rgba(217,217,217,1)_0%,rgba(217,217,217,1)_100%)]" />

      <div className="absolute top-[955px] left-[161px] w-[1269px] [font-family:'Inter-Black',Helvetica] font-black text-white text-8xl tracking-[0] leading-[normal]">
        Onam celebration events
      </div>

      <div className="absolute top-[1458px] left-[387px] w-[668px] h-[168px] bg-[linear-gradient(0deg,rgba(10,125,52,0.68)_0%,rgba(10,125,52,0.68)_100%),linear-gradient(0deg,rgba(217,217,217,1)_0%,rgba(217,217,217,1)_100%)]" />

      <div className="absolute top-[1242px] left-[574px] w-[280px] [font-family:'Inria_Serif-Bold',Helvetica] font-bold text-white text-8xl tracking-[0] leading-[normal]">
        Login
      </div>

      <div className="absolute top-[1479px] left-[508px] w-[443px] [font-family:'Inria_Serif-Bold',Helvetica] font-bold text-white text-8xl tracking-[0] leading-[normal]">
        Register
      </div>

      <div className="absolute top-[2136px] left-0 w-[1564px] h-52 bg-[#d9d9d9]" />

      <div className="absolute top-[2223px] left-[111px] w-[1099px] [font-family:'Inria_Serif-Bold',Helvetica] font-bold text-black text-8xl tracking-[0] leading-[normal] whitespace-nowrap">
        Vinodhini&nbsp;&nbsp;M k -25012248
      </div>
    </div>
  );
};
```
```
2nd page

import React from "react";
import onameve1 from "./onameve-1.png";
import star1 from "./star-1.svg";
import star2 from "./star-2.svg";
import star3 from "./star-3.svg";
import star4 from "./star-4.svg";
import star5 from "./star-5.svg";
import star6 from "./star-6.svg";

export const Frame = (): JSX.Element => {
  const events = [
    {
      id: 1,
      name: "Pookalam",
      top: "345px",
      icon: star1,
      iconHeight: "90px",
      iconWidth: "95px",
      textWidth: "513px",
    },
    {
      id: 2,
      name: "Chenda melam",
      top: "560px",
      icon: star2,
      iconHeight: "102px",
      iconWidth: "95px",
      textWidth: "873px",
    },
    {
      id: 3,
      name: "Traditional dances",
      top: "819px",
      icon: star3,
      iconHeight: "99px",
      iconWidth: "95px",
      textWidth: "1014px",
    },
    {
      id: 4,
      name: "Onam sadhya",
      top: "1056px",
      icon: star4,
      iconHeight: "99px",
      iconWidth: "95px",
      textWidth: "785px",
    },
    {
      id: 5,
      name: "Tug-of-war",
      top: "1280px",
      icon: star5,
      iconHeight: "95px",
      iconWidth: "95px",
      textWidth: "685px",
    },
    {
      id: 6,
      name: "DJ",
      top: "1506px",
      icon: star6,
      iconHeight: "95px",
      iconWidth: "95px",
      textWidth: "232px",
    },
  ];

  return (
    <div className="bg-white overflow-hidden w-full min-w-[1460px] min-h-[2460px] relative">
      <header className="absolute top-[-22px] left-[-34px] w-[1494px] h-[278px] bg-[linear-gradient(0deg,rgba(255,25,28,0.89)_0%,rgba(255,25,28,0.89)_100%),linear-gradient(0deg,rgba(217,217,217,1)_0%,rgba(217,217,217,1)_100%)]">
        <h1 className="absolute top-[59px] left-[97px] w-[1323px] [font-family:'Cherry_Bomb_One-Regular',Helvetica] font-normal text-white text-8xl tracking-[0] leading-[normal]">
          Onam celebration events
        </h1>
      </header>

      <main>
        <section aria-label="Event list">
          <ul className="list-none">
            {events.map((event) => (
              <li
                key={event.id}
                className="absolute"
                style={{ top: event.top, left: "139px" }}
              >
                <img
                  className="inline-block"
                  style={{ height: event.iconHeight, width: event.iconWidth }}
                  alt=""
                  src={event.icon}
                  aria-hidden="true"
                />
                <span
                  className="inline-block [font-family:'Cherry_Cream_Soda-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
                  style={{
                    width: event.textWidth,
                    marginLeft: event.id === 1 ? "197px" : "165px",
                  }}
                >
                  {event.name}
                </span>
              </li>
            ))}
          </ul>
        </section>

        <figure className="absolute top-[1694px] left-0 w-[1460px] h-[766px]">
          <img
            className="w-full h-full aspect-[1.84]"
            alt="Onam celebration illustration showing traditional boat, King Mahabali, and pookalam flower arrangement"
            src={onameve1}
          />
        </figure>
      </main>
    </div>
  );
};
```
```
3rd page
 
 import React, { useState } from "react";
import mahabali1 from "./mahabali-1.png";
import sadhya1 from "./sadhya-1.png";

export const Frame = (): JSX.Element => {
  const [formData, setFormData] = useState({
    fullName: "",
    gender: "",
    age: "",
    registerNo: "",
    department: "",
    mobileNo: "",
    emailId: "",
    eventsRegistered: "",
  });

  const handleInputChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    const { name, value } = e.target;
    setFormData((prev) => ({
      ...prev,
      [name]: value,
    }));
  };

  const handleSubmit = (e: React.FormEvent) => {
    e.preventDefault();
    console.log("Form submitted:", formData);
  };

  return (
    <div className="bg-white w-full min-w-[1234px] min-h-[2223px] relative">
      <header className="absolute top-0 left-0 w-[1234px] h-[279px] bg-[linear-gradient(0deg,rgba(101,19,169,0.88)_0%,rgba(101,19,169,0.88)_100%),linear-gradient(0deg,rgba(217,217,217,1)_0%,rgba(217,217,217,1)_100%)]">
        <h1 className="absolute top-[84px] left-[78px] w-[1083px] [font-family:'Inter-Regular',Helvetica] font-normal text-white text-8xl tracking-[0] leading-[normal]">
          Event Registration Form
        </h1>
      </header>

      <form onSubmit={handleSubmit}>
        <div className="absolute top-[377px] left-[60px] w-[624px] h-[132px] bg-[#d9d9d9]">
          <label
            htmlFor="fullName"
            className="absolute top-0 left-[80px] w-[458px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
          >
            Full name
          </label>
          <input
            type="text"
            id="fullName"
            name="fullName"
            value={formData.fullName}
            onChange={handleInputChange}
            className="absolute inset-0 w-full h-full bg-transparent px-[80px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
            aria-label="Full name"
            required
          />
        </div>

        <div className="absolute top-[572px] left-[60px] w-[624px] h-[125px] bg-[#d9d9d9]">
          <label
            htmlFor="gender"
            className="absolute top-0 left-[84px] w-[328px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
          >
            Gender
          </label>
          <input
            type="text"
            id="gender"
            name="gender"
            value={formData.gender}
            onChange={handleInputChange}
            className="absolute inset-0 w-full h-full bg-transparent px-[84px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
            aria-label="Gender"
            required
          />
        </div>

        <div className="absolute top-[763px] left-[60px] w-[624px] h-[122px] bg-[#d9d9d9]">
          <label
            htmlFor="age"
            className="absolute top-0 left-[84px] w-56 [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
          >
            Age
          </label>
          <input
            type="number"
            id="age"
            name="age"
            value={formData.age}
            onChange={handleInputChange}
            className="absolute inset-0 w-full h-full bg-transparent px-[84px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
            aria-label="Age"
            required
          />
        </div>

        <div className="absolute top-[962px] left-[60px] w-[624px] h-[126px] bg-[#d9d9d9]">
          <label
            htmlFor="registerNo"
            className="absolute top-0 left-[27px] w-[662px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
          >
            Register No:
          </label>
          <input
            type="text"
            id="registerNo"
            name="registerNo"
            value={formData.registerNo}
            onChange={handleInputChange}
            className="absolute inset-0 w-full h-full bg-transparent px-[27px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
            aria-label="Register Number"
            required
          />
        </div>

        <div className="absolute top-[1150px] left-[60px] w-[624px] h-[119px] bg-[#d9d9d9]">
          <label
            htmlFor="department"
            className="absolute top-0 left-[39px] w-[572px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
          >
            Department
          </label>
          <input
            type="text"
            id="department"
            name="department"
            value={formData.department}
            onChange={handleInputChange}
            className="absolute inset-0 w-full h-full bg-transparent px-[39px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
            aria-label="Department"
            required
          />
        </div>

        <div className="absolute top-[1331px] left-[60px] w-[624px] h-[133px] bg-[#d9d9d9]">
          <label
            htmlFor="mobileNo"
            className="absolute top-[18px] left-[59px] w-[522px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
          >
            Mobile No
          </label>
          <input
            type="tel"
            id="mobileNo"
            name="mobileNo"
            value={formData.mobileNo}
            onChange={handleInputChange}
            className="absolute inset-0 w-full h-full bg-transparent px-[59px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
            aria-label="Mobile Number"
            required
          />
        </div>

        <div className="absolute top-[1527px] left-[60px] w-[624px] h-[132px] bg-[#d9d9d9]">
          <label
            htmlFor="emailId"
            className="absolute top-0 left-[84px] w-[435px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
          >
            Email ID
          </label>
          <input
            type="email"
            id="emailId"
            name="emailId"
            value={formData.emailId}
            onChange={handleInputChange}
            className="absolute inset-0 w-full h-full bg-transparent px-[84px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-8xl tracking-[0] leading-[normal]"
            aria-label="Email ID"
            required
          />
        </div>

        <div className="absolute top-[1736px] left-[71px] w-[613px] h-[129px] bg-[#d9d9d9]">
          <label
            htmlFor="eventsRegistered"
            className="absolute top-[24px] left-[48px] w-[571px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-[64px] tracking-[0] leading-[normal]"
          >
            Events Registered
          </label>
          <input
            type="text"
            id="eventsRegistered"
            name="eventsRegistered"
            value={formData.eventsRegistered}
            onChange={handleInputChange}
            className="absolute inset-0 w-full h-full bg-transparent px-[48px] [font-family:'Secular_One-Regular',Helvetica] font-normal text-black text-[64px] tracking-[0] leading-[normal]"
            aria-label="Events Registered"
            required
          />
        </div>

        <button
          type="submit"
          className="absolute top-[1983px] left-[227px] w-[478px] h-[143px] bg-[linear-gradient(0deg,rgba(227,22,22,0.96)_0%,rgba(227,22,22,0.96)_100%),linear-gradient(0deg,rgba(217,217,217,1)_0%,rgba(217,217,217,1)_100%)] cursor-pointer hover:opacity-90 transition-opacity"
          aria-label="Submit form"
        >
          <span className="absolute top-[24px] left-[53px] w-[368px] [font-family:'Inter-Regular',Helvetica] font-normal text-white text-8xl tracking-[0] leading-[normal]">
            SUBMIT
          </span>
        </button>
      </form>

      <img
        className="absolute top-[1683px] left-[751px] w-[452px] h-[451px] aspect-[1] object-cover"
        alt="Mahabali"
        src={mahabali1}
      />

      <img
        className="absolute top-[349px] left-[671px] w-[563px] h-[396px] aspect-[1.5] object-cover"
        alt="Sadhya"
        src={sadhya1}
      />
    </div>
  );
};
```

## OUTPUT:
![alt text](<Screenshot (40).png>)

## RESULT:
The program to design, develop and deploy a web application for event registration using Figma UI tool is completed successfully.
