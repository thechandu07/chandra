// script.js
const projects = [
  {
    title: "Hospital Management System",
    description: "A comprehensive system for managing hospital operations.",
    link: "#"
  },
  {
    title: "Cafe Management System",
    description: "Manage cafe orders and reservations with a QR-based system.",
    link: "#"
  },
  {
    title: "Stock Trading App",
    description: "A demo app for managing stock trades and tracking prices.",
    link: "#"
  }
];

const projectList = document.getElementById("project-list");
projects.forEach((project) => {
  const projectDiv = document.createElement("div");
  projectDiv.innerHTML = `
    <h3>${project.title}</h3>
    <p>${project.description}</p>
    <a href="${project.link}" target="_blank">View Project</a>
  `;
  projectList.appendChild(projectDiv);
});
