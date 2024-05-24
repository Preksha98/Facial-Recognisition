This project involves developing a facial recognition system to facilitate employee entry scanning using features of the left and right sides of the face. The system leverages OpenCV's CascadeClassifier for real-time face detection and recognition.

Key Components:

Face Detection with CascadeClassifier:

Utilize OpenCV's pre-trained Haar cascades or LBP cascades to detect faces in real-time.
Detect the face by analyzing the image frame-by-frame from the video feed.
Separate detection for the left and right profiles to ensure accurate recognition even if the face is partially turned.
Data Collection and Preprocessing:

Collect a dataset of employee facial images, ensuring varied angles, lighting, and expressions.
Preprocess the images by converting them to grayscale to simplify the computation and improve detection accuracy.
Augment the dataset with left and right profile images of each employee.
Training the Classifier:

Train the classifier using the collected dataset to recognize distinct facial features of each employee.
Implement feature extraction techniques to focus on unique facial landmarks.
Face Recognition:

Extract facial features from the detected faces and compare them against the stored features in the database.
Use a suitable recognition algorithm (e.g., Eigenfaces, Fisherfaces, or LBPH) to match the detected face with the employee database.
Ensure recognition works accurately for left and right profiles.
Entry Scanning System:

Integrate the face recognition system with the entry gate mechanism.
Implement real-time recognition where the system checks the detected face against the database and grants access if a match is found.
Ensure the system can handle real-time entry of multiple employees with minimal delay.
