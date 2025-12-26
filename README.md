/* ===== Reset and base styles ===== */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  line-height: 1.6;
  background-color: #fff8f0;
  color: #4e342e; /* coklat gelap */
  scroll-behavior: smooth;
}

a {
  text-decoration: none;
  color: inherit;
}

img {
  max-width: 100%;
  display: block;
}

/* Container max width */
.container {
  width: 90%;
  max-width: 1100px;
  margin: 0 auto;
}

/* ===== Navbar ===== */
nav {
  background-color: #f5e9dc; /* krem */
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  position: sticky;
  top: 0;
  z-index: 100;
}

nav .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 0;
}

.logo {
  font-weight: 700;
  font-size: 1.5rem;
  font-style: italic;
  letter-spacing: 1px;
  color: #6d4c41; /* coklat medium */
  cursor: default;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 1.8rem;
}

nav ul li a {
  font-weight: 500;
  font-size: 1rem;
  color: #6d4c41;
  transition: color 0.3s ease;
}

nav ul li a:hover,
nav ul li a:focus {
  color: #a1887f; /* coklat terang */
}

/* ===== Hero Section ===== */
#hero {
  background-color: #f7f0e9; /* krem lebih terang */
  text-align: center;
  padding: 4rem 1rem 6rem;
  color: #4e342e;
}

#hero h1 {
  font-size: 2.8rem;
  font-weight: 700;
  margin-bottom: 0.3rem;
}

#hero p {
  font-size: 1.3rem;
  font-weight: 300;
  margin-bottom: 2rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
  font-style: italic;
}

#hero .btn {
  background-color: #6d4c41;
  color: #fff;
  padding: 0.8rem 2.2rem;
  border: none;
  border-radius: 25px;
  font-weight: 600;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

#hero .btn:hover,
#hero .btn:focus {
  background-color: #8d6e63;
  outline: none;
}

/* ===== Sections common styles ===== */
section {
  padding: 4rem 1rem;
}

h2.section-title {
  text-align: center;
  font-size: 2rem;
  font-weight: 700;
  margin-bottom: 2rem;
  color: #5d4037;
  letter-spacing: 1px;
}

p.section-text {
  max-width: 700px;
  margin: 0 auto 2rem;
  font-weight: 400;
  font-size: 1.1rem;
  color: #6f4e37;
  text-align: center;
  line-height: 1.5;
}

/* ===== Tentang Kami Section ===== */
#tentang .value-list {
  max-width: 600px;
  margin: 0 auto;
  font-size: 1rem;
  line-height: 1.5;
  color: #6f4e37;
  font-style: italic;
}

/* ===== Menu Section ===== */
#menu .card-container {
  max-width: 900px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
  gap: 1.4rem;
}

#menu .card {
  background-color: #f5e9dc;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(109, 76, 65, 0.2);
  padding: 1rem 1.2rem;
  text-align: center;
  cursor: default;
  transition: transform 0.2s ease;
  user-select: none;
}

#menu .card:hover {
  transform: translateY(-5px);
}

#menu .card h3 {
  font-size: 1.2rem;
  color: #4e342e;
  font-weight: 600;
}

/* ===== Galeri Section ===== */
#galeri .gallery-grid {
  max-width: 1000px;
  margin: 0 auto;
  display: grid;
  gap: 1rem;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  border-radius: 12px;
  overflow: hidden;
}

#galeri .gallery-grid img {
  width: 100%;
  height: 140px;
  object-fit: cover;
  border-radius: 8px;
  box-shadow: 0 1px 4px rgba(109, 76, 65, 0.3);
  transition: transform 0.3s ease;
  cursor: pointer;
}

#galeri .gallery-grid img:hover {
  transform: scale(1.05);
}

/* ===== Lokasi & Kontak Section ===== */
#kontak {
  background-color: #f7f0e9;
  max-width: 700px;
  margin: 0 auto;
  text-align: center;
  color: #5d4037;
  font-size: 1.1rem;
  line-height: 1.6;
}

#kontak p {
  margin: 0.6rem 0;
}

#kontak .label {
  font-weight: 700;
  margin-right: 0.5rem;
  color: #6d4c41;
}

/* ===== Footer ===== */
footer {
  background-color: #6d4c41;
  color: #f5e9dc;
  text-align: center;
  padding: 1.2rem 0;
  font-size: 0.95rem;
}

/* ===== Responsive Navbar for smaller screens ===== */
@media (max-width: 720px) {
  nav .container {
    flex-direction: column;
    gap: 0.8rem;
  }
  nav ul {
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
  }
  #hero h1 {
    font-size: 2rem;
  }
  #hero p {
    font-size: 1rem;
  }
  #menu .card-container {
    grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
  }
  #galeri .gallery-grid img {
    height: 120px;
  }
}
