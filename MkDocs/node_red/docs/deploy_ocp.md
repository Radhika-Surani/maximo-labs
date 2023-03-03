## Deploy Node-RED in the OpenShift Container Platorm (OCP)

1. Login to OpenShift
2. Home -> Projects
3. Create Project called node-red
<br>
![Create project](/img/node_red/create_project.png)

4. Switch to the Developer role
<br>
![Developer role](/img/node_red/developer_role.png)

5. Click on +Add
<br>
![Add to project](/img/node_red/add_to_project.png)

6. Click on Import from Git
7. Enter Git Repo URL https://github.com//node-red/node-red-docker 
8. Scroll down to Advanced options
9. Enter Target port 1880
<br>
![Target port](/img/node_red/target_port.png)

10. Click Create
11. Click on the blue D for Deployment
12. See Build #1 is running
<br>
![Target port](/img/node_red/build_running.png)

13. Wait a few minutes for the build of the container
14. Check that the Pod is in Running state
<br>
![Pod running](/img/node_red/pod_running.png)

15. Click on the arrow to launch Node-RED
<br>
![Launch Node-RED](/img/node_red/node_red_launch.png)

16. Welcome to Node-RED
<br>
![Node-RED Welcome](/img/node_red/node_red_welcome.png)


## Add required additional nodes

* node-red-dashboard
* node-red-contrib-ui-upload
* node-red-contrib-chunks-to-lines
* node-red-nodes-cf-sqldb-dashdb

<br>
1. Click on the burger menu in upper right hand corner and select Manage palette
<br>
![Manage palette](/img/node_red/manage_palette.png)

2. Click on Install and enter node-red-dashboard in the Search field - then click on Install
<br>
![Node red dashboard](/img/node_red/node_red_dashboard.png)

3. Click on Install again
<br>
![Node red dashboard](/img/node_red/installing.png)

4. Wait until you see the new nodes have been installed
![Node red dashboard](/img/node_red/nodes_added_to_palette.png)

5. Repeat step 2-4 for the other 3 libraries
