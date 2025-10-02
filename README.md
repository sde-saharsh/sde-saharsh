<h1 align="center">Hi 👋, I'm Saharsh Khalokar</h1>
<h3 align="center">A Passionate Full-Stack Developer & Problem Solver</h3>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=25&pause=1000&center=true&vCenter=true&width=500&lines=Welcome+to+my+GitHub!;Full-Stack+Developer;MERN+Stack+Enthusiast;Problem+Solver;Lifelong+Learner" alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=your-github-username&style=flat-square&color=blue" alt="Visitor Counter" />
</p>

---

## 🚀 About Me
- 🌱 Currently learning **MERN Stack (MongoDB, Express.js, React.js, Node.js)**
- 🎯 My goal is to **master full-stack development** and contribute to open-source projects.
- 💡 I love building creative projects and solving real-world problems.
- 📈 Always passionate about growth and continuous learning.


---



<p align="center">
  💬 *Let’s Connect and Build Something Amazing Together!*
</p>
import { cn } from "@/lib/utils";
import React from "react";
import { motion } from "framer-motion";
import { FaArrowDown } from 'react-icons/fa';

import {
  FaReact,
  FaNodeJs,
  FaDatabase,
  FaCloud,
  FaLaptopCode,
} from "react-icons/fa";
import { SiMongodb, SiFrontendmentor } from "react-icons/si";
import { BiCodeAlt } from "react-icons/bi";

const techStack = [
  { icon: <FaCloud />, label: "Cloud" },
  { icon: <SiFrontendmentor />, label: "Frontend" },
  { icon: <BiCodeAlt />, label: "Full-Stack" },
  { icon: <FaNodeJs />, label: "Node.js" },
  { icon: <FaReact />, label: "React" },
  { icon: <FaDatabase />, label: "Database" },
  { icon: <FaLaptopCode />, label: "Backend" },
  { icon: <FaCloud />, label: "Cloud" },
  { icon: <SiFrontendmentor />, label: "Frontend" },
  { icon: <BiCodeAlt />, label: "Full-Stack" },
  { icon: <FaNodeJs />, label: "Node.js" },
  { icon: <FaReact />, label: "React" },
  { icon: <FaDatabase />, label: "Database" },
  { icon: <FaLaptopCode />, label: "Backend" },
  { icon: <FaCloud />, label: "Cloud" },
  { icon: <SiFrontendmentor />, label: "Frontend" },
  { icon: <BiCodeAlt />, label: "Full-Stack" },
  { icon: <FaNodeJs />, label: "Node.js" },
  { icon: <FaReact />, label: "React" },
  { icon: <FaDatabase />, label: "Database" },
  { icon: <FaLaptopCode />, label: "Backend" },
  { icon: <FaCloud />, label: "Cloud" },
  { icon: <SiFrontendmentor />, label: "Frontend" },
  { icon: <BiCodeAlt />, label: "Full-Stack" },
  { icon: <FaNodeJs />, label: "Node.js" },
  { icon: <FaReact />, label: "React" },
  { icon: <FaDatabase />, label: "Database" },
  { icon: <FaLaptopCode />, label: "Backend" },
];

export function GridBackgroundDemo() {
  return (
    <div className="relative flex h-screen w-full items-center justify-center bg-black overflow-hidden">
      {/* Grid background */}
      <div
        className={cn(
          "absolute inset-0",
          "[background-size:80px_80px]",
          "[background-image:linear-gradient(to_right,#262626_1px,transparent_1px),linear-gradient(to_bottom,#262626_1px,transparent_1px)]"
        )}
      />

      {/* Spotlight overlay */}
      <div className="pointer-events-none absolute inset-0 flex items-center justify-center [mask-image:radial-gradient(ellipse_at_center,transparent_20%,black)] dark:bg-black" />

      {/* Main content */}
      <div className="flex flex-col items-center justify-center h-full px-4 text-white relative z-10">
        {/* Scroll Down Indicator */}
        <div className="text-center mt-10">
          <p className="text-sm sm:text-base text-white">
            Scroll down for more information...
          </p>

          <div className="md:w-100 h-[1px] bg-[#a6a6a6] mx-auto my-4" />

          <div className="w-15 h-15 sm:w-12 sm:h-12 mx-auto rounded-full bg-gray-500 flex items-center justify-center animate-bounce cursor-pointer mt-8">
            <FaArrowDown className="text-black text-lg" />
          </div>
        </div>
      </div>

      {/* Tech stack marquee */}
      <div className="absolute bottom-0 right-0 w-full bg-black py-4 mt-12">
        {/* Top Row: Scroll Left */}
        <div className="marquee-wrapper">
          <div className="marquee-track">
            {[...techStack, ...techStack].map((item, i) => (
              <div
                key={`top-${i}`}
                className="flex items-center gap-2 text-white text-base sm:text-lg px-4 min-w-max"
              >
                {item.icon}
                <span>{item.label}</span>
              </div>
            ))}
          </div>
        </div>

        {/* Bottom Row: Scroll Right */}
        <div className="marquee-wrapper mt-4">
          <div className="marquee-track reverse">
            {[...techStack, ...techStack].map((item, i) => (
              <div
                key={`bottom-${i}`}
                className="flex items-center gap-2 text-white text-base sm:text-lg px-4 min-w-max"
              >
                {item.icon}
                <span>{item.label}</span>
              </div>
            ))}
          </div>
        </div>
      </div>
    </div>
  );
}
