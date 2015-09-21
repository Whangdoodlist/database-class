# database-class
Part 4
SELECT loc_id, bldg_code, room, capacity
FROM location
ORDER BY loc_id;

SELECT f_id, f_last, f_first, f_mi, loc_id, f_phone, f_rank, f_super, f_pin, f_image
FROM faculty
ORDER BY f_id;

SELECT s_id, s_last, s_first, s_mi, s_address, s_city, s_state, s_zip, s_phone, s_class, s_dob, s_pin, f_id, time_enrolled
FROM student
ORDER BY s_last;

SELECT term_id, term_desc, status, start_date
FROM term
ORDER BY term_id;

SELECT course_id, course_no, course_name, credits
FROM course
ORDER BY course_id;

SELECT c_sec_id, course_id, term_id, sec_num, f_id, c_sec_day, c_sec_time, c_sec_duration, loc_id
FROM course_section
ORDER BY c_sec_id;

SELECT s_id, c_sec_id, grade
FROM enrollment
ORDER BY s_id;
