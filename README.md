Commands:
python -m virtualenv venv 
cd venv/Scripts   
./activate   
$env:FLASK_App = "app"  
pip install -r requirements.txt
flask run 
deactivate  


Why I used :
flasgger
flask_restx
flask_sqlalchemy
flask_jwt_extended
