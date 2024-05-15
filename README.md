# radio-sq-cu
finding square and cube of a nnmber
Imports System.Runtime.CompilerServices
Imports System.Runtime.Serialization
Imports System.Windows.Forms.VisualStyles.VisualStyleElement.Button

Public Class Form1
    Private Sub Form1_Load(sender As Object, e As EventArgs) Handles MyBase.Load
        Label1.Text = "SELECT YOUR CHOICE"
        Label2.Text = "Enter a number"
        RadioButton1.Text = "Square"
        RadioButton2.Text = "Cube"
        Button1.Text = "Submit"
    End Sub

    Private Sub Button1_Click(sender As Object, e As EventArgs) Handles Button1.Click
        Dim a, c, d As Integer
        a = TextBox1.Text
        c = a * a
        d = a * a * a
        If RadioButton1.Checked = True Then
            MsgBox("Square is" & c)
        End If
        If RadioButton2.Checked = True Then
            MsgBox("Cube is" & d)
        End If
    End Sub
End Class
