# masengkelle-portfolio
Portfolio Website Masengkelle
import { useState } from "react";

const classes = {
  page: "min-h-screen bg-gray-900 text-gray-100 px-6 py-10",
  container: "max-w-4xl mx-auto",
  avatarWrapper: "flex justify-center",
  avatar: "w-40 h-40 rounded-xl object-cover shadow-lg",
  name: "text-3xl font-bold mt-4 text-center",
  role: "text-gray-400 text-center",
  section: "mt-10",
  sectionTitle: "text-xl font-semibold mb-4 text-blue-300",
  card: "bg-gray-800 p-5 rounded-xl shadow-md",
  chip: "px-3 py-1 bg-gray-700 rounded-full text-sm",
  btn: "px-4 py-2 bg-blue-500 hover:bg-blue-600 text-white rounded-lg text-sm font-semibold inline-block",
};

export default function App() {
  return (
    <div className={classes.page}>
      <div className={classes.container}>

        {/* Foto Profil */}
        <div className={classes.avatarWrapper}>
          <img
            src="https://drive.google.com/uc?export=view&id=1rkpxrodyXi7C-PGV-LsNk17icsdlENWZ"
            alt="Aji Januakto Wibowo"
            className={classes.avatar}
          />
        </div>

        {/* Nama & Role */}
        <h1 className={classes.name}>Aji Januakto Wibowo (Masengkelle)</h1>
        <p className={classes.role}>Mahasiswa • Palu</p>

        {/* Tentang */}
        <div className={classes.section}>
          <h2 className={classes.sectionTitle}>Tentang Saya</h2>
          <div className={classes.card}>
            <p className="text-gray-300">
              Saya memiliki pengalaman sebagai sales di PT Home Credit Indonesia 
              (Maret–Nov 2024) dengan pencapaian pembiayaan hingga 75jt. Saat ini 
              saya fokus belajar Web Development.
            </p>
          </div>
        </div>

        {/* Kontak */}
        <div className={classes.section}>
          <h2 className={classes.sectionTitle}>Kontak</h2>
          <div className={classes.card + " space-y-2"}>
            <p>📞 Telepon: 0852-4209-9970</p>
            <p>📧 Email: mass12mass11@gmail.com</p>
            <p>🌐 Website: https://masengkelle.com</p>
            <p>🔗 LinkedIn: linkedin.com/in/aji januakto wibowo</p>

            <a href="https://wa.me/6285242099970" target="_blank" className={classes.btn}>
              WhatsApp
            </a>
          </div>
        </div>

        {/* Keahlian */}
        <div className={classes.section}>
          <h2 className={classes.sectionTitle}>Keahlian</h2>
          <div className="flex flex-wrap gap-2">
            {["Komunikasi", "HTML", "CSS", "JavaScript", "Microsoft"].map((skill) => (
              <span key={skill} className={classes.chip}>{skill}</span>
            ))}
          </div>
        </div>

      </div>
    </div>
  );
}
