package sample;

import javafx.application.Application;
import javafx.fxml.FXMLLoader;
import javafx.scene.Parent;
import javafx.scene.Scene;
import javafx.scene.layout.Pane;
import javafx.stage.Stage;

public class Main extends Application {

    public static String name = "";
    public static int rounds = 0;
    public static int questionsPerRound = 0;

    public void init() {
        Controller.readProperties();

    }

    @Override
    public void start(Stage primaryStage) throws Exception {

        System.out.println(name);
        System.out.println(rounds);
        System.out.println(questionsPerRound);

        try {
            FXMLLoader loader = new FXMLLoader(getClass().getResource("sample.fxml"));
            loader.setController(new Controller());
            Pane root = loader.load();
            Scene scene = new Scene(root, 800, 800);
            primaryStage.setScene(scene);
            primaryStage.show();
        }catch (Exception e){
            e.printStackTrace();
        }
    }

    public static void main(String[] args) {
        launch(args);
    }
}
