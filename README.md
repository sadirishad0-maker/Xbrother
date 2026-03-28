# Xbrother
# Example: Fair candidate selection system  applicants = [     {"name": "Ayesha", "skills": ["Python", "Django"], "gender": "Female"},     {"name": "Rahim", "skills": ["JavaScript", "React"], "gender": "Male"},     {"name": "Sumi", "skills": ["Python", "Flask"], "gender": "Female"} ]  def select_candidates(applicants, required_skill)
function updateProfile() {
  const pass = document.getElementById('adminPass').value;
  const newName = document.getElementById('newName').value;
  const newEmail = document.getElementById('newEmail').value;
  const newPicUrl = document.getElementById('newPicUrl').value;

  if(pass === "admin123") {
    if(newName) document.getElementById('profileName').innerText = newName;
    if(newEmail) document.getElementById('profileEmail').innerHTML = "<strong>Email:</strong> " + newEmail;
    if(newPicUrl) document.getElementById('profilePic').src = newPicUrl;
    alert("✅ Profile updated by admin.");
  } else {
    alert("❌ Access denied. Only admin can change profile details.");
  }
}
