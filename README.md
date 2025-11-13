import React from "react";

const Portfolio: React.FC = () => {
  return (
    <div className="min-h-screen bg-gradient-to-b from-slate-50 via-white to-slate-50 text-slate-900 antialiased">
      {/* HEADER / HERO */}
      <header className="relative bg-[linear-gradient(90deg,#0f172a_0%,#071029_100%)] text-white">
        <div className="max-w-6xl mx-auto px-6 py-20 flex flex-col-reverse md:flex-row items-center gap-10">
          <div className="w-full md:w-1/2">
            <h1 className="text-4xl md:text-5xl font-extrabold leading-tight">Amberose Gill</h1>
            <p className="mt-4 text-lg opacity-90">Mechanical Engineer • CFD / FEA • Simulation-driven design</p>
            <p className="mt-6 text-sm max-w-lg opacity-80">
              BEng Mechanical Engineering. I design, simulate, and build: Tesla turbines, aerodynamic analyses and engineering systems — using ANSYS, SolidWorks and Python.
            </p>
            <div className="mt-6 flex flex-wrap gap-3">
              <a href="#projects" className="inline-block bg-cyan-500 hover:bg-cyan-600 text-white px-4 py-2 rounded-md text-sm font-medium">View Projects</a>
              <a href="#contact" className="inline-block border border-white/20 hover:bg-white/5 text-white px-4 py-2 rounded-md text-sm">Contact</a>
              <a href="/AMBEROSE GILL CV.pdf" className="inline-block ml-2 text-sm underline">Download CV</a>
            </div>
          </div>
          <div className="w-full md:w-1/2 flex justify-center">
            <div className="w-80 h-80 rounded-2xl bg-gradient-to-br from-slate-800 via-cyan-800 to-indigo-900 shadow-2xl p-6 relative overflow-hidden">
              <svg className="absolute inset-0 w-full h-full opacity-30" viewBox="0 0 600 600" fill="none" xmlns="http://www.w3.org/2000/svg">
                <g stroke="url(#g)" strokeWidth="1">
                  <path d="M20 120 C150 10, 450 10, 580 120" strokeOpacity="0.25" />
                  <path d="M20 200 C150 90, 450 90, 580 200" strokeOpacity="0.18" />
                </g>
              </svg>
              <div className="relative z-10 text-white flex flex-col items-center justify-center h-full">
                <div className="bg-white/5 rounded-full px-4 py-2 text-xs font-semibold">Tesla Turbine • Ø254 mm • 50 discs</div>
                <div className="mt-6 text-center max-w-xs">
                  <h3 className="text-xl font-bold">Small-scale Tesla Turbine</h3>
                  <p className="mt-2 text-xs opacity-90">Experimental output 180 W — validated with CFD and analytical models.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </header>

      {/* ABOUT */}
      <section id="about" className="max-w-6xl mx-auto px-6 py-12 grid md:grid-cols-3 gap-8 items-center">
        <div className="md:col-span-2">
          <h2 className="text-2xl font-semibold">About</h2>
          <p className="mt-4 text-lg text-slate-700">Mechanical Engineering graduate with hands-on experience in CAD, CFD and FEA simulations using ANSYS and SolidWorks.</p>
          <ul className="mt-6 grid sm:grid-cols-2 gap-3 text-sm text-slate-600">
            <li>• ANSYS Fluent / CFX • FEA (Mechanical & Thermal)</li>
            <li>• SolidWorks / Creo • CAD & fabrication</li>
            <li>• Python / C++ • automation</li>
          </ul>
        </div>
        <div className="bg-white rounded-lg shadow p-6">
          <h3 className="font-medium">Quick facts</h3>
          <div className="mt-4 text-sm text-slate-600 space-y-2">
            <div><strong>Degree:</strong> BEng Mechanical Engineering — NUST</div>
            <div><strong>Location:</strong> Sialkot, Pakistan</div>
            <div><strong>Interests:</strong> CFD, Turbomachinery, Experimental testing</div>
          </div>
        </div>
      </section>

      {/* PROJECTS */}
      <section id="projects" className="max-w-6xl mx-auto px-6 py-12">
        <h2 className="text-2xl font-semibold">Projects</h2>
        <div className="mt-6 grid md:grid-cols-2 gap-6">
          <article className="bg-white rounded-xl p-6 shadow hover:shadow-lg transition">
            <h3 className="font-bold text-lg">Design, Analysis & Fabrication of Small-Scale Tesla Turbine</h3>
            <p className="mt-2 text-sm text-slate-700">Ø254 mm, 50-discs. Experimental power 180 W, theoretical 254 W. CFD validation with k–ω SST.</p>
          </article>
          <article className="bg-white rounded-xl p-6 shadow hover:shadow-lg transition">
            <h3 className="font-bold text-lg">Airfoil Aerodynamic Analysis</h3>
            <p className="mt-2 text-sm text-slate-700">NACA 0012, 2412 — angle-of-attack studies, pressure coefficient validation and mesh independence tests.</p>
          </article>
        </div>
      </section>

      {/* EXPERIENCE */}
      <section id="experience" className="max-w-6xl mx-auto px-6 py-12">
        <h2 className="text-2xl font-semibold">Experience</h2>
        <div className="mt-6 space-y-4">
          <div className="p-4 rounded-lg border">
            <h3 className="font-semibold">CFD Engineer (Freelancer) — Fiverr</h3>
            <p className="mt-2 text-sm text-slate-700">Delivered 10+ CFD projects on ANSYS Fluent; aerodynamic analyses for various airfoils and turbomachinery.</p>
          </div>
          <div className="p-4 rounded-lg border">
            <h3 className="font-semibold">Intern — InspecTest (NDT)</h3>
            <p className="mt-2 text-sm text-slate-700">Hands-on experience with PT, MPT and UT following standard safety protocols.</p>
          </div>
        </div>
      </section>

      {/* EDUCATION & CERTIFICATIONS */}
      <section id="education" className="max-w-6xl mx-auto px-6 py-12 grid md:grid-cols-2 gap-6">
        <div>
          <h2 className="text-2xl font-semibold">Education</h2>
          <div className="mt-4 p-4 rounded-lg border">
            <h3 className="font-semibold">BEng Mechanical Engineering — NUST</h3>
            <p className="mt-2 text-sm text-slate-700">Thesis: Design, Analysis and Fabrication of Small-Scale Tesla Turbine</p>
          </div>
        </div>
        <div>
          <h2 className="text-2xl font-semibold">Certifications</h2>
          <div className="mt-4 p-4 rounded-lg border space-y-2 text-sm text-slate-700">
            <div>• ANSYS: Applications of Shock Expansion</div>
            <div>• ANSYS: Turbulence Modeling in Fluent</div>
            <div>• ANSYS: Vertical Axis Wind Turbine</div>
          </div>
        </div>
      </section>

      {/* CONTACT */}
      <section id="contact" className="max-w-6xl mx-auto px-6 py-12">
        <h2 className="text-2xl font-semibold">Contact</h2>
        <div className="mt-6 grid md:grid-cols-2 gap-6">
          <div className="p-6 rounded-lg border">
            <h3 className="font-semibold">Get in touch</h3>
            <p className="mt-2 text-sm text-slate-700">Email me at <a href="mailto:amberosegill@gmail.com" className="underline">amberosegill@gmail.com</a></p>
          </div>
          <div className="p-6 rounded-lg border">
            <h3 className="font-semibold">Quick links</h3>
            <ul className="mt-3 text-sm text-slate-700 space-y-2">
              <li><a href="https://www.linkedin.com/in/amberose-gill-070a9422a/" className="underline">LinkedIn</a></li>
              <li><a href="https://www.fiverr.com/zerose_1?public_mode=true" className="underline">Fiverr</a></li>
              <li><a href="/AMBEROSE GILL CV.pdf" className="underline">Download CV</a></li>
            </ul>
          </div>
        </div>
      </section>

      <footer className="bg-slate-900 text-white py-6">
        <div className="max-w-6xl mx-auto px-6 flex flex-col md:flex-row justify-between items-center gap-4">
          <div className="text-sm">© {(new Date()).getFullYear()} Amberose Gill — Mechanical Engineering Portfolio</div>
          <div className="text-sm opacity-80">Built with React + Tailwind</div>
        </div>
      </footer>
    </div>
  );
};

export default Portfolio;
