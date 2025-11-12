

```VB
Public Function calculaSuma(valor1 As Integer, valor2 As Integer) As Integer
    calculaSuma = valor1 + valor2
End Function


Public Function calculaResta(valor1 As Integer, valor2 As Integer) As Integer
    calculaResta = valor1 - valor2
End Function

Public Function calculaMulti(valor1 As Integer, valor2 As Integer) As Integer
    calculaMulti = valor1 * valor2
End Function

Public Function calculaDivision(Numerador As Integer, Denominador As Integer) As Double
    Dim a
    Sheets("Hoja1").Select
    If Denominador > 0 Then
        calculaDivision = Numerador / Denominador
    Else
        a = MsgBox("El resultado de la division no puede ser cero", , "Division")
    End If
End Function

'GENERACIÓN DE SUBRUTINAS'

Public Sub tareaSub()
    Sheets("Hoja1").Select
    Cells(1, 1) = "Hola mundo"
    Range(Cells(2, 6), Cells(3, 6)) = "Hola mundo con un rango de (2,3)(3,6)"
    Range("A3:A6") = "Excel"
End Sub

Public Function Divf() As Double

    Dim a
    Dim num As Integer
    Dim den As Integer
    
    num = InputBox("Ingrese el numerador", "División")
    den = InputBox("Ingrese el denominador", "División")
    Divf = num / den
    a = MsgBox("El resultado de la división es " & Divf, "División")
    
End Function

Public Sub DivS()
    Dim a
    Dim num As Integer
    Dim den As Integer

    num = InputBox("Ingrese el numerador", "División")
    den = InputBox("Ingrese el denominador", "División")
    
    a = MsgBox("El resultado de la división es " & num / dev, , "División")
    
End Sub


'GENERACIÓN DE CONDICIONALES Select Case'

Public Function CondicionalSC(numA As Integer, numB As Integer, numC As Integer) As String
    Dim suma As Integer
    
    suma = numA + numB + numC
    
    Select Case suma
        Case Is < 0
            CondicionalSC = "Negativo"
        Case Is = 0
            CondicionalSC = "Cero"
        Case Is > 0
            CondicionalSC = "Positivo"
        Case Else
            CondicionalSC = "Ni Idea que demonios metiste"
    End Select
End Function

Public Sub ClasificarEdad()

    Dim edad As Integer
    
    edad = InputBox("Ingresa tu edad:", "Clasificación de Edad")
    
    Select Case edad
    
    Case 0 To 12
    
    MsgBox "Eres un niño"
    
    Case 13 To 17
    
    MsgBox "Eres un adolescente"
    
    Case 18 To 59
    
    MsgBox "Eres un adulto"
    
    Case 60 To 99
    
    MsgBox "Eres un adulto mayor"
    
    Case Else
    
    MsgBox "Edad inválida"
    
    End Select

End Sub

Public Function dado() As String

    Dim VD As Integer
    Dim a
    VD = Int((Rnd * 6) + 1)
    
    If VD = 2 Then
            dado = "Par"
        ElseIf VD = 4 Then
            dado = "Par"
        ElseIf VD = 6 Then
            dado = "Par"
        Else
            dado = "ImPar"
    End If
    a = MsgBox(VD, , "Dado")
End Function

```