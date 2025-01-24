# SQL-Comic-Book-Database


This repository contains the files and resources for the Comic Book Database project, developed as part of the ISE 305 course. The project aims to provide a platform for comic book enthusiasts to manage their collections and access detailed information on titles, issues, authors, characters, and publishers.

## Project Overview

The Comic Book Database project was designed to:
- Allow users to input and manage comic book details, such as title, issue number, publication date, authors, artists, and synopsis.
- Support categorization by genre (e.g., superheroes, fantasy, horror) and publisher (e.g., Marvel, DC).
- Utilize MySQL Workbench for schema design and MS Access for database implementation and hierarchical forms.
- Enable complex queries and relationships reflecting real-world comic book data.

### Team Members
- **Edward Yeboah:** Data retrieval, query creation, and discussion on relationships.
- **Naolin Ramos:** Entity attributes, foreign key designations, and PowerPoint slide preparation.
- **Synia Grimes:** Form and report creation, PowerPoint slide editing.

---

## Features

### **Entities**
- **Comic Titles:** Stores information about the comic titles, their genres, and publishers.
- **Issues:** Includes data about specific issues of each title, such as issue number, publication date, and synopsis.
- **Characters:** Tracks characters appearing in comic books, including their roles and affiliations.
- **Writers and Artists:** Details creative teams behind each issue, including cover artists.
- **Publishers:** Information about publishers like Marvel and DC.

### **Relationships**
- **One-to-Many:**
  - Publishers → Comic Titles
  - Comic Titles → Issues
- **Many-to-Many:**
  - Characters ⇄ Issues
  - Writers ⇄ Issues
  - Issues ⇄ Cover Artists

### **Forms**
Hierarchical forms in MS Access allow users to:
- View comic titles and related issues in parent-child forms.
- Explore writers and their contributions to specific issues.

### **Key Queries**
1. Retrieve all characters and their alignment (hero/villain).
2. List characters appearing in specific issues (e.g., "House of Mystery #301").
3. Show all writers and the issues they contributed to.
4. List all cover artists for issues published by DC.
5. Find issues released before February 2008 along with their writers.

---

## Requirements

- **Tools:**
  - MS Access (for database and forms)
  - MySQL Workbench (for schema design)
- **Data Source:**
  - Kaggle datasets containing comic book titles, character appearances, and creative team information.

---

## How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/<your-username>/ComicBookDatabase.git
   cd ComicBookDatabase
   ```

2. **Open the database in MS Access:**
   - Use `project_database.accdb` to explore tables, queries, forms, and reports.

3. **View the relational data model:**
   - Open `database_model.mwb` in MySQL Workbench.

4. **Run SQL scripts:**
   - Use `queries.sql` to create tables, insert data, and execute queries.

5. **Explore hierarchical forms:**
   - Open MS Access forms (e.g., Comic Titles → Issues) to interact with parent-child relationships.

---

## Future Improvements

- Refactor the database to minimize redundancy in junction tables (e.g., `characters_has_issues` and `writers_has_issues`).
- Expand the dataset to include more publishers and genres.
- Implement user authentication for personalized collections.

---

## Authors
- **Edward Yeboah**
- **Naolin Ramos**
- **Synia Grimes**

---

## License
This project is licensed under the MIT License.

