package com.Mygame;

import javax.swing.*;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.util.Currency;
import java.util.Locale;

public class CurrencyConvertor {
    public static void main(String[] args) {
        JFrame ff = new JFrame("currencyConvertor ");
        ff.setVisible(false);
       // Frame f = new Frame("CurrencyConvertor");
//        f.setLayout(null);
//
//        f.setBounds(20,20,600,600);
//        f.setBackground(Color.red);
        ff.setLayout(null);
       // f.setVisible(true);

        ff.setBounds(20,20,600,600);
        JLabel l1 = new JLabel("Welcom to my currency convertor ");
        l1.setBounds(180,50,200,30);
        ff.add(l1);
        JLabel l2 = new JLabel("enter your currency in rupees .....");
        l2.setBounds(100,150,200,30);
        ff.add(l2);
        JTextField t1 = new JTextField();

        t1.setBounds(320,150,200,30);
        t1.setVisible(true);
        t1.setBackground(Color.yellow);
        ff.add(t1);
        JButton b = new JButton("Convertor ");
        b.setLayout(null);
        b.setBounds(180,450,200,30);
        ff.add(b);
        JLabel l3 = new JLabel();
        JLabel l4 = new JLabel();
        JLabel l5 = new JLabel();
        l3.setBounds(130,200,300,30);
        ff.add(l3);
        l4.setBounds(130,250,300,30);
        ff.add(l4);
        l5.setBounds(130,300,300,30);
        ff.add(l5);
        Currency cu = Currency.getInstance(Locale.UK);
        Currency cc = Currency.getInstance(Locale.CHINA);

       b.addActionListener(new ActionListener() {
           @Override
           public void actionPerformed(ActionEvent e) {
               ff.setVisible(false);
               JFrame f1 = new JFrame();
               f1.setLayout(null);
               f1.setBounds(20,20,800,800);
               Float x = Float.parseFloat(t1.getText());
               f1.add(l1);

               f1.add(l2);
               l3.setText("The given rupees in dollar is ..   $"+(x*0.012));
               f1.add(l3);
               l4.setText("The given rupees in pound is ..  "+cu.getSymbol()+" "+(x*0.012));
               f1.add(l4);
               l5.setText("The given rupees in yuan is ..  "+cc.getSymbol()+" "+(x*0.084));
               f1.add(l5);
               f1.add(t1);
               f1.add(b);
               f1.setVisible(true);
           }
       });



        ff.setVisible(true);

        //f.add(l1);

    }
}
