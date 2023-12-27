 if (reg.Text == "")

 {
     string querry = "INSERT INTO info VALUES('" + reg.Text + "','" + fname.Text + "', '" + lname.Text + "', '" + dateTimePicker1.Value.ToString() + "','" + gend + "', '" + addr.Text + "', '" + email.Text + "', '" + pno.Text + "', '" + eno.Text + "', '" + pfname.Text + "', '" + plname.Text + "', '" + pnic.Text + "', '" + pcono.Text + "')";

     SqlCommand cmd = new SqlCommand(querry, Con);
     cmd.ExecuteNonQuery();
     MessageBox.Show("Information Successfully Added!");
 }
