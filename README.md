A set of tools that can be used to ease grading.

Workflow:

	mkdir assignment_name
	mv mycourses_dump.zip assignment_name
	cd assignment_name
	unzip mycourses_dump.zip
	# Remove the old versions
	cleanup .
	# Unzip each zip into the base files
	prepare .
	# Move each student's files into a directory for that student
	folderize .
	# Create a config for the grading GUI
	cd ..
	mkdir -p rules
	vim rules/assignment_name.txt
	# Fill with data as specified in the grade utility
	grade assignment_name

