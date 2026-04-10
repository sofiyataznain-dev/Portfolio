// 🚀 ULTRA PRO PORTFOLIO (ENHANCED CONTENT)
// Only content upgraded as requested

import { motion } from "framer-motion";
import { useState } from "react";

export default function App() {
  return (
    <div className="bg-gradient-to-b from-black via-gray-900 to-black text-white min-h-screen scroll-smooth">
      <Navbar />
      <Hero />
      <About />
      <Skills />
      <Experience />
      <Projects />
      <Contact />
    </div>
  );
}

function Navbar() {
  return (
    <nav className="fixed w-full top-0 bg-black/40 backdrop-blur-md z-50 flex justify-between px-6 py-4">
      <h1 className="font-bold text-lg">Sofiya</h1>
      <div className="flex gap-6 text-sm">
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </div>
    </nav>
  );
}

function Hero() {
  return (
    <section className="h-screen flex flex-col justify-center items-center text-center px-4">
      <motion.h1
        initial={{ opacity: 0, y: -50 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 1 }}
        className="text-5xl md:text-7xl font-bold"
      >
        Sofiya Taznain
      </motion.h1>

      <motion.p
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ delay: 0.5 }}
        className="mt-4 text-lg md:text-2xl text-gray-400"
      >
        AI/ML Developer | Building Intelligent Systems
      </motion.p>

      <div className="mt-6 flex gap-4">
        <a href="#projects" className="bg-white text-black px-6 py-2 rounded-xl hover:scale-105 transition">
          View Work
        </a>
        <a href="#contact" className="border px-6 py-2 rounded-xl hover:scale-105 transition">
          Contact
        </a>
      </div>
    </section>
  );
}

// 🔥 UPDATED ABOUT (LONGER + STRONG)
function About() {
  return (
    <section id="about" className="py-20 px-6 md:px-20 text-center">
      <h2 className="text-3xl font-bold mb-6">About Me</h2>
      <p className="text-gray-400 max-w-3xl mx-auto leading-relaxed">
        I am an AI/ML Developer passionate about building intelligent, scalable, and impactful systems that solve real-world problems. With hands-on experience in machine learning, deep learning, and full-stack development, I focus on creating solutions that combine data-driven insights with practical applications.
        <br /><br />
        I have worked on developing predictive models, computer vision systems, and data analytics dashboards that improve decision-making and efficiency. My approach involves not just building models, but optimizing them for performance, scalability, and usability in real environments.
        <br /><br />
        Alongside AI, I enjoy working with modern web technologies like React and Node.js to integrate machine learning into user-friendly applications. I am continuously learning and exploring new advancements in Generative AI, data science, and system design to stay ahead in the tech space.
      </p>
    </section>
  );
}

function Skills() {
  const skills = [
    "Python","TensorFlow","PyTorch","React","Node.js","SQL","MongoDB","Docker","Power BI"
  ];

  return (
    <section className="py-20 px-6 md:px-20">
      <h2 className="text-3xl font-bold text-center mb-10">Skills</h2>
      <div className="grid grid-cols-2 md:grid-cols-4 gap-6">
        {skills.map((s, i) => (
          <div key={i} className="bg-gray-900 p-6 rounded-xl text-center hover:scale-110 hover:shadow-xl hover:shadow-white/10 transition">
            {s}
          </div>
        ))}
      </div>
    </section>
  );
}

function Experience() {
  return (
    <section className="py-20 px-6 md:px-20">
      <h2 className="text-3xl font-bold text-center mb-10">Experience</h2>

      <div className="space-y-8">
        <Card title="AI/ML Developer" subtitle="Future Education | 2025" points={[
          "Improved model accuracy by 15%",
          "Built CNN models with 94% F1-score",
          "Reduced training latency by 20%"
        ]} />

        <Card title="Data Analyst" subtitle="Meadowkart | 2024–2025" points={[
          "Analyzed 10K+ records",
          "Saved 5+ hrs/week",
        ]} />
      </div>
    </section>
  );
}

function Card({ title, subtitle, points }) {
  return (
    <div className="bg-gray-900 p-6 rounded-xl hover:scale-[1.02] transition">
      <h3 className="text-xl font-semibold">{title}</h3>
      <p className="text-gray-400">{subtitle}</p>
      <ul className="list-disc ml-6 mt-2 text-gray-300">
        {points.map((p, i) => <li key={i}>{p}</li>)}
      </ul>
    </div>
  );
}

// 🔥 UPDATED PROJECTS (FULL + TOOLS)
function Projects() {
  const [selected, setSelected] = useState(null);

  const projects = [
    {
      title: "AI Image Classification System",
      desc: "Deep learning-based multi-class image classifier",
      details: "Developed a Convolutional Neural Network (CNN) model to classify images across 50+ categories with high accuracy. Implemented preprocessing pipelines and optimized training performance.",
      tools: "TensorFlow, Python, NumPy, OpenCV"
    },
    {
      title: "Sales Forecasting Model",
      desc: "Predictive analytics model for business forecasting",
      details: "Built a machine learning model to forecast sales trends using historical data. Achieved low MAE and improved decision-making for business planning.",
      tools: "Scikit-learn, Pandas, Python, Matplotlib"
    },
    {
      title: "Cybersecurity Threat Detection System",
      desc: "Anomaly detection system for security threats",
      details: "Designed a system to detect abnormal patterns in network data to identify potential threats. Improved detection accuracy significantly.",
      tools: "Python, Machine Learning, Data Analysis"
    }
  ];

  return (
    <section id="projects" className="py-20 px-6 md:px-20">
      <h2 className="text-3xl font-bold text-center mb-10">Projects</h2>

      <div className="grid md:grid-cols-3 gap-6">
        {projects.map((p, i) => (
          <div key={i} onClick={() => setSelected(p)} className="bg-gray-900 p-6 rounded-xl cursor-pointer hover:scale-105 transition">
            <h3 className="text-xl font-semibold">{p.title}</h3>
            <p className="text-gray-400">{p.desc}</p>
          </div>
        ))}
      </div>

      {selected && (
        <div className="fixed inset-0 bg-black/80 flex justify-center items-center">
          <div className="bg-gray-900 p-6 rounded-xl max-w-md">
            <h3 className="text-xl font-bold">{selected.title}</h3>
            <p className="mt-2 text-gray-400">{selected.details}</p>
            <p className="mt-3 text-sm text-gray-500">Tools: {selected.tools}</p>
            <button onClick={() => setSelected(null)} className="mt-4 bg-white text-black px-4 py-2 rounded">Close</button>
          </div>
        </div>
      )}
    </section>
  );
}

// 🔥 CONTACT WITH LINKS
function Contact() {
  return (
    <section id="contact" className="py-20 px-6 md:px-20 text-center">
      <h2 className="text-3xl font-bold mb-6">Contact</h2>
      <p className="text-gray-400">taznainsofiya@gmail.com</p>

      <div className="mt-6 flex justify-center gap-6">
        <a href="https://www.linkedin.com/in/sofiya-taznain-540a08321?utm_source=share_via&utm_content=profile&utm_medium=member_android" target="_blank" className="underline">LinkedIn</a>
        <a href="https://github.com/sofiyataznain-dev" target="_blank" className="underline">GitHub</a>
      </div>
    </section>
  );
}

// 🎯 NOW THIS IS A STRONG PORTFOLIO

