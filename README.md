Chapter4_Challenge_DiaryManager

Project Name: Chapter4_Challenge_DiaryManager
Language: Java
Topic: Chapter 4 – File I/O, BufferedReader/BufferedWriter, and File Management

Project Overview

The Personal Diary Manager is a command-line diary application designed to:

Write personal diary entries

Read previous entries

Search entries by keyword

Backup all entries as a ZIP file

Optionally save application state using serialization

Each diary entry is saved as a separate text file with a timestamp in the filename for organization and easy retrieval.

This project demonstrates practical use of Java I/O operations, Files API, menu-driven programs, exception handling, and object serialization.

Features
1. Entry Management

Each diary entry is saved as:
diary_YYYY_MM_DD_HH_MM_SS.txt

Uses LocalDateTime and DateTimeFormatter for timestamps

Entries are stored in the entries/ folder

2. Core Functionality

Write Mode:
Prompt the user for diary text and save it to a new file

Read Mode:
List all entries and allow the user to select one to read

Search Mode:
Search entries containing a specific keyword

Backup Mode:
Create a ZIP archive of all diary entries

3. Technical Implementation

Text Operations: Uses BufferedReader and BufferedWriter

File Management: Uses java.nio.file.Files API for directory and file handling

Menu System: Simple menu-driven interface for user interaction

Exception Handling: Graceful handling of all possible I/O errors

4. Advanced Features (Bonus)

Serialization: Save last opened entry or last searched keyword to diary_config.ser

Backup: ZIP archive of all diary entries for safety and portability
