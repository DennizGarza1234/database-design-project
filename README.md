# database-design-project

This database design organizes key entities involved in managing a sports team, including Stakeholders, Players, Coaches, Games, Attendance, Performance Stats, and Notifications. The primary design decision was to centralize all people-related data under the Stakeholders table to maintain consistency and enable flexible roles. Players and Coaches reference Stakeholders via foreign keys, ensuring data integrity.

Challenges included managing foreign key relationships and ensuring referential integrity, especially when inserting sample data with interconnected tables. Balancing normalization with usability led to a clear separation of game-related data and performance statistics. The UNIQUE constraint on jersey numbers ensures no duplicate player identifiers, though this required careful sample data generation.

Overall, this design aims for scalability, data accuracy, and ease of maintenance to support efficient team management and detailed game analytics.
