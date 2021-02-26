# Four_Action_button
import java.awt.*;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class checkbox {
    checkbox() {
        Checkbox N;
        Checkbox E;
        Checkbox b;
        Checkbox s;

        Frame f=new Frame("checkbox");
        f.setLayout(null);
        f.setVisible(true);
        f.setSize(600,500);
//        f.setBackground(Color.red);
        N=new Checkbox("NAME",true);
        E=new Checkbox("ENROLLMENT",);
        b=new Checkbox("BRANCH",);
        s=new Checkbox("SUBJECT",);
        N.setBounds(20,40,80,30);
        E.setBounds(20,60,80,30);
        b.setBounds(20,80,80,30);
        s.setBounds(20,100,80,30);
        f.add(N);
        f.add(E);
        f.add(b);
        f.add(s);

        f.addWindowListener(new WindowAdapter() {
            public void windowClosing(WindowEvent we) {
                System.exit(0);

            }
        });


    }
    public static void main(String[] args) {
        new checkbox();
    }
}
