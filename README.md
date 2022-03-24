# mvp_pattern
MVP_Pattern 공부

view -> presenter : userAction 
presenter -> view : Update UI
Model -> presenter : Model Update 
presenter -> Model : Update Model

mvp는 model과 view, presenter로 나누는 패턴이다. 
mvc와 비교하여 view와 model이 서로 존재를 몰라 의존성이 떨어진다.

Model : LocalDB, RemoteDB, SharedPreference 등 데이터를 수정,관리하는 클래스 
presenter : 사용자의 액션을 받아 로직을 처리, Model에게 Data 변경 요구 UI업데이트 하는 로직을 처리하는 Class
View : 사용자의 액션을 Presenter에 떠넘기고, UI업데이트를 하는 코드만 있는 클래스 

view : Activity , Fragment 같은 View이다. 
model : Retrofit2를 사용하는 곳 
