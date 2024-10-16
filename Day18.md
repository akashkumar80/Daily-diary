# Day 18:-5 July 2024

## GUI Programming using JavaFX
JavaFX is a Java library that is used to develop Desktop applications as well as Rich Internet Applications (RIA). The applications built in JavaFX, can run on multiple platforms including Web, Mobile and Desktops.

### Install Eclipse
In order to run the JavaFX application, we need to set up eclipse.
Download the eclipse from it's website and follow the instruction which we have done on day2.

### Example
```java
package application;   
import javafx.application.Application;  
import javafx.event.ActionEvent;  
import javafx.event.EventHandler;  
import javafx.scene.Scene;  
import javafx.scene.control.Button;  
import javafx.stage.Stage;  
import javafx.scene.layout.StackPane;  
public class Hello_World extends Application{  
  
    @Override  
    public void start(Stage primaryStage) throws Exception {  
        // TODO Auto-generated method stub  
        Button btn1=new Button("Say, Hello World");  
        btn1.setOnAction(new EventHandler<ActionEvent>() {  
              
            @Override  
            public void handle(ActionEvent arg0) {  
                // TODO Auto-generated method stub  
                System.out.println("hello world");  
            }  
        });  
        StackPane root=new StackPane();  
        root.getChildren().add(btn1);  
        Scene scene=new Scene(root,600,400);      
        primaryStage.setTitle("First JavaFX Application");  
        primaryStage.setScene(scene);  
        primaryStage.show();  
    }  
    publicstaticvoid main (String[] args)  
    {  
        launch(args);  
    }  
  
}  
```