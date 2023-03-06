public class JavaCalculator extends javax.swing.JFrame {

    double firstNum;
    double secondNum;
    double total;
    double plusminus;

    int plusClick;
    int minusClick;
    int multiplyClick;
    int devideClick;
    int decimalClick;


   
    public JavaCalculator() {
        initComponents();
    }


 private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
    display.setText(display.getText()+jButton1.getText());
    }                                        

    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
     display.setText(display.getText()+jButton2.getText());
    }                                        

    private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {                                         
     display.setText(display.getText()+jButton3.getText());
    }                                        

    private void jButton4ActionPerformed(java.awt.event.ActionEvent evt) {                                         
     display.setText(display.getText()+jButton4.getText());
    }                                        

    private void jButton5ActionPerformed(java.awt.event.ActionEvent evt) {                                         
     display.setText(display.getText()+jButton5.getText());
    }                                        

    private void jButton6ActionPerformed(java.awt.event.ActionEvent evt) {                                         
     display.setText(display.getText()+jButton6.getText());
    }                                        

    private void jButton7ActionPerformed(java.awt.event.ActionEvent evt) {                                         
     display.setText(display.getText()+jButton7.getText());
    }                                        

    private void jButton8ActionPerformed(java.awt.event.ActionEvent evt) {                                         
     display.setText(display.getText()+jButton8.getText());
    }                                        

    private void Button9ActionPerformed(java.awt.event.ActionEvent evt) {                                        
     display.setText(display.getText()+Button9.getText());
    }                                       

    private void jButton10ActionPerformed(java.awt.event.ActionEvent evt) {                                          
     display.setText(display.getText()+jButton10.getText());
    }                                         

    private void decimalActionPerformed(java.awt.event.ActionEvent evt) {                                        
     if(decimalClick==0){
        display.setText(display.getText()+decimal.getText());
        decimalClick=1;
    }                                       
    }
    private void clearActionPerformed(java.awt.event.ActionEvent evt) {                                      
     display.setText("");
     decimalClick=0;
    }                                     

    private void posnegActionPerformed(java.awt.event.ActionEvent evt) {                                       
    plusminus=(Double.parseDouble(String.valueOf(display.getText())));
    plusminus=plusminus*(-1);
    display.setText(String.valueOf(plusminus));
    }                                      

    private void plusActionPerformed(java.awt.event.ActionEvent evt) {                                     
     firstNum=(Double.parseDouble(String.valueOf(display.getText())));
     display.setText("");
     plusClick=1;
     decimalClick=0;
    }                                    

    private void minusActionPerformed(java.awt.event.ActionEvent evt) {                                      
     firstNum=(Double.parseDouble(String.valueOf(display.getText())));
     display.setText("");
     minusClick=1;
     decimalClick=0;
    }                                     

    private void multiplyActionPerformed(java.awt.event.ActionEvent evt) {                                         
     firstNum=(Double.parseDouble(String.valueOf(display.getText())));
     display.setText("");
     multiplyClick=1;
     decimalClick=0;
    }                                        

    private void divideActionPerformed(java.awt.event.ActionEvent evt) {                                       
     firstNum=(Double.parseDouble(String.valueOf(display.getText())));
     display.setText("");
     devideClick=1;
     decimalClick=0;
    }                                      

    private void equalsActionPerformed(java.awt.event.ActionEvent evt) {                                       
     secondNum=(Double.parseDouble(String.valueOf(display.getText())));
     if(plusClick>0){
     total = firstNum + secondNum;
     display.setText(String.valueOf(total));
     firstNum = 0;
     secondNum = 0;
     plusClick = 0;
     }


     if(minusClick>0){
     total = firstNum - secondNum;
     display.setText(String.valueOf(total));
     firstNum = 0;
     secondNum = 0;
     minusClick = 0;

    }                                      
    
     if(multiplyClick>0){
     total = firstNum * secondNum;
     display.setText(String.valueOf(total));
     firstNum = 0;
     secondNum = 0;
     multiplyClick = 0;
     
    }

     if(devideClick>0){
     total = firstNum / secondNum;
     display.setText(String.valueOf(total));
     firstNum = 0;
     secondNum = 0;
     devideClick = 0;

    }
    }
    
    public static void main(String args[]) {
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new JavaCalculator().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify                     
    private javax.swing.JButton Button9;
    private javax.swing.JButton clear;
    private javax.swing.JButton decimal;
    private javax.swing.JTextField display;
    private javax.swing.JButton divide;
    private javax.swing.JButton equals;
    private javax.swing.JButton jButton1;
    private javax.swing.JButton jButton10;
    private javax.swing.JButton jButton2;
    private javax.swing.JButton jButton3;
    private javax.swing.JButton jButton4;
    private javax.swing.JButton jButton5;
    private javax.swing.JButton jButton6;
    private javax.swing.JButton jButton7;
    private javax.swing.JButton jButton8;
    private javax.swing.JButton jButton9;
    private javax.swing.JPanel jPanel1;
    private javax.swing.JButton minus;
    private javax.swing.JButton multiply;
    private javax.swing.JButton plus;
    private javax.swing.JButton posneg;
    // End of variables declaration                   

}