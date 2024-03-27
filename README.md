# DoPrzero
<Window x:Class="sudoku.MainWindow"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
        xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
        xmlns:local="clr-namespace:sudoku"
        mc:Ignorable="d"
        Title="MainWindow" Height="450" Width="800">
    <Window.Resources>
        <Style x:Key="SudokuButtonStyle" TargetType="Button">
            <Setter Property="Width" Value="50"/>
            <Setter Property="Height" Value="50"/>
            <Setter Property="FontSize" Value="20"/>
        </Style>
        <Style x:Key="CheckButtonStyle" TargetType="Button">
            <Setter Property="Width" Value="100"/>
            <Setter Property="Height" Value="50"/>
            <Setter Property="FontSize" Value="20"/>
            <Setter Property="Background" Value="#FF4CAF50"/>
            <Setter Property="Foreground" Value="White"/>
            <Setter Property="BorderThickness" Value="2"/>
            <Setter Property="BorderBrush" Value="#FF388E3C"/>
            <Setter Property="HorizontalAlignment" Value="Center"/>
            <Setter Property="VerticalAlignment" Value="Center"/>
        </Style>
    </Window.Resources>
    <Grid Margin="20">
        <TabControl>
            <TabItem Header="4x4">
                <UniformGrid Rows="5" Columns="4" Margin="10" x:Name="sudokuGrid">
                    <Button  Margin="5" Click="Button_Click" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_1" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_2" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_3" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_4" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_5" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_6" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_7" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_8" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_9" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_10" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_11" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_12" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_13" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_14" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button  Margin="5" Click="Button_Click_15" Style="{StaticResource SudokuButtonStyle}"/>
                    <Button Content="Sprawdź" Margin="5" Click="Button_Click_16" Style="{StaticResource CheckButtonStyle}"/>
                </UniformGrid>
            </TabItem>
        </TabControl>
    </Grid>
</Window>



using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows;
using System.Windows.Controls;
using System.Windows.Controls.Primitives;
using System.Windows.Data;
using System.Windows.Documents;
using System.Windows.Input;
using System.Windows.Media;
using System.Windows.Media.Imaging;
using System.Windows.Navigation;
using System.Windows.Shapes;

namespace sudoku
{
   
    public partial class MainWindow : Window
    {
        public MainWindow()
        {
            InitializeComponent();
        }

        private void Button_Click(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());
                
                if(ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_1(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_2(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_3(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_4(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_5(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_6(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_7(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_8(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_9(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_10(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_11(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_12(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_13(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_14(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private void Button_Click_15(object sender, RoutedEventArgs e)
        {
            Button button = (Button)sender;
            if (button.Content == null)
            {
                button.Content = "1";
            }
            else
            {
                int ile = Int32.Parse(button.Content.ToString());

                if (ile == 4)
                {
                    ile = 1;
                }
                else
                {
                    ile++;
                }
                button.Content = ile.ToString();
            }
        }

        private bool CheckSudoku()
        {
            // Sprawdzanie poprawności wierszy
            for (int row = 0; row < 4; row++)
            {
                HashSet<string> rowValues = new HashSet<string>();
                for (int col = 0; col < 4; col++)
                {
                    Button button = GetButtonAt(row, col);
                    if (button.Content == null)
                        return false; // Gra nie jest kompletna

                    string content = button.Content.ToString();
                    if (!rowValues.Add(content))
                        return false; // Duplikat w wierszu
                }
            }

            // Sprawdzanie poprawności kolumn
            for (int col = 0; col < 4; col++)
            {
                HashSet<string> colValues = new HashSet<string>();
                for (int row = 0; row < 4; row++)
                {
                    Button button = GetButtonAt(row, col);
                    string content = button.Content.ToString();
                    if (!colValues.Add(content))
                        return false; // Duplikat w kolumnie
                }
            }

            // Sprawdzanie poprawności małych kwadratów 2x2
            for (int startRow = 0; startRow < 4; startRow += 2)
            {
                for (int startCol = 0; startCol < 4; startCol += 2)
                {
                    HashSet<string> squareValues = new HashSet<string>();
                    for (int row = startRow; row < startRow + 2; row++)
                    {
                        for (int col = startCol; col < startCol + 2; col++)
                        {
                            Button button = GetButtonAt(row, col);
                            string content = button.Content.ToString();
                            if (!squareValues.Add(content))
                                return false; // Duplikat w małym kwadracie 2x2
                        }
                    }
                }
            }

            return true; // Wszystkie warunki są spełnione - Sudoku jest poprawnie uzupełnione
        }

        private Button GetButtonAt(int row, int col)
        {
            // Pobieranie przycisku na podstawie współrzędnych w siatce 4x4
            foreach (var child in sudokuGrid.Children)
            {
                if (child is UniformGrid grid && Grid.GetRow(grid) == row && Grid.GetColumn(grid) == col)
                {
                    foreach (var button in grid.Children)
                    {
                        if (button is Button)
                        {
                            return (Button)button;
                        }
                    }
                }
            }
            return null;
        }


        private void Button_Click_16(object sender, RoutedEventArgs e)
        {
            bool isValid = CheckSudoku(); // Wywołanie funkcji sprawdzającej poprawność gry Sudoku
            if (isValid)
            {
                // Wyświetlenie okienka informacyjnego o poprawnym uzupełnieniu Sudoku
                MessageBox.Show("Gratulacje! Sudoku jest poprawnie uzupełnione.", "Sudoku", MessageBoxButton.OK, MessageBoxImage.Information);
            }
            else
            {
                // Wyświetlenie okienka ostrzegawczego o błędnym uzupełnieniu Sudoku
                MessageBox.Show("Niestety, Sudoku jest źle uzupełnione. Spróbuj jeszcze raz.", "Sudoku", MessageBoxButton.OK, MessageBoxImage.Error);
            }
        }
    }
}
