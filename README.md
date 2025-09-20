A hospital Booking System that allows patients of different hospitals to book appointments with specific doctors.

To acccess the website via link: https://medbook1.onrender.com

To download the code and run it locally on your machine follow the instructions below:

1) Create a directory on Desktop
2) Download the repo inside the directory
3) Navigate to the folder directory and create a venv using  python -m venv venv
4) Activate the venv using venv\Scripts\Activate
5) Run pip install -r requirements.txt to install the dependencies
6) Run waitress-serve --listen=0.0.0.0:5000 table:app to run the backend locally
7) Access the website via link or from the html files in directory (need to change the API calls to localhost/5000 if accessed html files from directory)
