
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
    <meta name="description" content="">
    <meta name="google" content="notranslate">

      <script>
    window.dataLayer = window.dataLayer || [];
    dataLayer.push({"userId":205867,"visitorType":"student","batch":{"id":62,"fullNameWithC":"NBO-1122 (C#11)","schoolLocation":{"id":7,"name":"Nairobi"}},"curriculum":{"id":1,"name":"Foundations"}});

    window.gtm_user_custom_event = function (name, options) {
      if (typeof name === 'undefined') {
        return;
      }

      window.dataLayer.push({
        customEventOptions: typeof options !== 'undefined' ? options : {},
        event: name,
      });
    }
  </script>

  <!-- Google Tag Manager -->
  <script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
  new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
  j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
  'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
  })(window,document,'script','dataLayer','GTM-N4C8MF2');</script>
  <!-- End Google Tag Manager -->


    <title>Project: 0x05. Python - Exceptions | Nairobi Intranet</title>

      <link rel="stylesheet" href="https://use.typekit.net/xgz4ilr.css">
      <link rel="stylesheet" media="all" href="/assets/application_alx-21c3687a217e1b4f93a21d8f80373745796d1fc436898edc667eb90f4c5c9970.css" />
      <script src="https://www.gstatic.com/charts/loader.js"></script>
      <script src="/assets/application-28fbde0d9d7e01867b82fdb2a88556984777beb449e6fde74a7b722d6c9d640a.js"></script>
      <link rel="shortcut icon" type="image/x-icon" href="/favicon_alx.ico" />
      <meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="OzhETbh5S345pM3gWYTQ8lMwjQmKHJf2rPJ5nIhBrwkQDsf_Gc9nEU9gOVzdYHju-fcwcfW4Gs_iZhzujkxazQ" />

      <link rel="apple-touch-icon" href="/apple-touch-icon_alx.png">

      <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
      <!--[if lt IE 9]>
        <script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
        <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
      <![endif]-->

      <!-- Store user timezone -->
      <script>
        Cookies.set('timezone', (new Date()).getTimezoneOffset() / -60.0);
      </script>

      <!-- intro.js for interactive onboarding -->

      <!-- React -->
      <script src="/packs/js/application-3cba0ec82ab41d0f9ad5.js"></script>
      <link rel="stylesheet" media="screen" href="/packs/css/application-87456da7.css" />
  </head>

  <body class="signed_in env_production notranslate"
        translate="no"
        class="notranslate"
        data-theme-suffix="_alx">
      <!-- Google Tag Manager (noscript) -->
  <noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-N4C8MF2"
  height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
  <!-- End Google Tag Manager (noscript) -->


      <input type="hidden" id="hbtn-slack-url" value="https://alx-students.slack.com">
      <nav class="navbar navbar-default navbar-fixed-top topbar visible-xs">
  <div class="navbar-header">
    <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar-mobile" aria-expanded="false">
      <span class="sr-only">Toggle navigation</span>
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
    </button>

    <a class="navbar-brand" href="/">
      <div class="logo"></div>
</a>  </div>

  <div class="collapse navbar-collapse navigation" id="navbar-mobile">
    <ul class="nav navbar-nav">
      


    <li data-container="body" data-placement="right" data-toggle="tooltip" title="My Planning"><a href="/planning/me"><div class="icon "><i aria-hidden="true" class="fa fa-calendar "></i></div><div class="visible-xs">My Planning</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-current-projects-item" title="Projects"><a href="/projects/current"><div class="icon "><i aria-hidden="true" class="fa fa-code-fork "></i></div><div class="visible-xs">Projects</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="QA Reviews I can make"><a href="/corrections/to_review"><div class="icon "><i aria-hidden="true" class="fa fa-check "></i></div><div class="visible-xs">QA Reviews I can make</div></a></li>
    
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Evaluation quizzes"><a href="/dashboards/my_current_evaluation_quizzes"><div class="icon "><i aria-hidden="true" class="fa fa-question "></i></div><div class="visible-xs">Evaluation quizzes</div></a></li>

    <hr title="My resources">

    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Curriculums"><a href="/dashboards/my_curriculums"><div class="icon "><i aria-hidden="true" class="fa fa-graduation-cap "></i></div><div class="visible-xs">Curriculums</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-concepts-item" title="Concepts"><a href="/concepts"><div class="icon "><i aria-hidden="true" class="fa fa-file-text "></i></div><div class="visible-xs">Concepts</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-video-rooms" title="Conference rooms"><a href="/dashboards/video_rooms"><div class="icon "><i aria-hidden="true" class="fa fa-comments "></i></div><div class="visible-xs">Conference rooms</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Servers"><a href="/servers"><div class="icon "><i aria-hidden="true" class="fa fa-server "></i></div><div class="visible-xs">Servers</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-my-containers" title="Sandboxes"><a href="/user_containers/current"><div class="icon "><i aria-hidden="true" class="fa fa-terminal "></i></div><div class="visible-xs">Sandboxes</div></a></li>
    
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Video on demand"><a href="/dashboards/videos"><div class="icon "><i aria-hidden="true" class="fa fa-film "></i></div><div class="visible-xs">Video on demand</div></a></li>

      <hr title="My campus">

      
      <li data-container="body" data-placement="right" data-toggle="tooltip" title="Peers"><a href="/users/peers"><div class="icon "><i aria-hidden="true" class="fa fa-users "></i></div><div class="visible-xs">Peers</div></a></li>
      <li data-container="body" data-placement="right" data-toggle="tooltip" title="Captain&#39;s Logs"><a href="/dashboards/my_captain_log"><div class="icon "><i aria-hidden="true" class="fa fa-book "></i></div><div class="visible-xs">Captain&#39;s Logs</div></a></li>


<hr class="visible-xs">

<li>
    <div
      data-container="body"
      data-placement="right"
      data-toggle="tooltip"
      title="Slack">
      <a target="_blank" href="https://alx-students.slack.com">
        <div class="image slack">
          <div class="inner"></div>
        </div>
        <div class="visible-xs">Slack</div>
</a>    </div>

  <div
    data-container="body"
    data-placement="right"
    data-toggle="tooltip"
    title="My Profile">
    <a href="/users/my_profile">
        <div class="image ">
          <div class="inner" style="background-image: url('https://s3.amazonaws.com/alx-intranet.hbtn.io/users/photos/000/205/867/thumb/20221114_131346.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230420%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20230420T192350Z&amp;X-Amz-Expires=600&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=61fc4dfb5e6fd5b24a8d6b683f48d81422c6d399c5738d862ea9d224a14b3193')"></div>
        </div>

      <div class="visible-xs">My Profile</div>
</a>  </div>
</li>


    </ul>
  </div>
</nav>

      <div class="hidden-xs navigation sidebar">
  <a class="logo-container" href="/">
    <div class="logo"></div>
</a>
  <ul>
    


    <li data-container="body" data-placement="right" data-toggle="tooltip" title="My Planning"><a href="/planning/me"><div class="icon "><i aria-hidden="true" class="fa fa-calendar "></i></div><div class="visible-xs">My Planning</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-current-projects-item" title="Projects"><a href="/projects/current"><div class="icon "><i aria-hidden="true" class="fa fa-code-fork "></i></div><div class="visible-xs">Projects</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="QA Reviews I can make"><a href="/corrections/to_review"><div class="icon "><i aria-hidden="true" class="fa fa-check "></i></div><div class="visible-xs">QA Reviews I can make</div></a></li>
    
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Evaluation quizzes"><a href="/dashboards/my_current_evaluation_quizzes"><div class="icon "><i aria-hidden="true" class="fa fa-question "></i></div><div class="visible-xs">Evaluation quizzes</div></a></li>

    <hr title="My resources">

    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Curriculums"><a href="/dashboards/my_curriculums"><div class="icon "><i aria-hidden="true" class="fa fa-graduation-cap "></i></div><div class="visible-xs">Curriculums</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-concepts-item" title="Concepts"><a href="/concepts"><div class="icon "><i aria-hidden="true" class="fa fa-file-text "></i></div><div class="visible-xs">Concepts</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-video-rooms" title="Conference rooms"><a href="/dashboards/video_rooms"><div class="icon "><i aria-hidden="true" class="fa fa-comments "></i></div><div class="visible-xs">Conference rooms</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Servers"><a href="/servers"><div class="icon "><i aria-hidden="true" class="fa fa-server "></i></div><div class="visible-xs">Servers</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-my-containers" title="Sandboxes"><a href="/user_containers/current"><div class="icon "><i aria-hidden="true" class="fa fa-terminal "></i></div><div class="visible-xs">Sandboxes</div></a></li>
    
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Video on demand"><a href="/dashboards/videos"><div class="icon "><i aria-hidden="true" class="fa fa-film "></i></div><div class="visible-xs">Video on demand</div></a></li>

      <hr title="My campus">

      
      <li data-container="body" data-placement="right" data-toggle="tooltip" title="Peers"><a href="/users/peers"><div class="icon "><i aria-hidden="true" class="fa fa-users "></i></div><div class="visible-xs">Peers</div></a></li>
      <li data-container="body" data-placement="right" data-toggle="tooltip" title="Captain&#39;s Logs"><a href="/dashboards/my_captain_log"><div class="icon "><i aria-hidden="true" class="fa fa-book "></i></div><div class="visible-xs">Captain&#39;s Logs</div></a></li>


<hr class="visible-xs">

<li>
    <div
      data-container="body"
      data-placement="right"
      data-toggle="tooltip"
      title="Slack">
      <a target="_blank" href="https://alx-students.slack.com">
        <div class="image slack">
          <div class="inner"></div>
        </div>
        <div class="visible-xs">Slack</div>
</a>    </div>

  <div
    data-container="body"
    data-placement="right"
    data-toggle="tooltip"
    title="My Profile">
    <a href="/users/my_profile">
        <div class="image ">
          <div class="inner" style="background-image: url('https://s3.amazonaws.com/alx-intranet.hbtn.io/users/photos/000/205/867/thumb/20221114_131346.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230420%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20230420T192350Z&amp;X-Amz-Expires=600&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=61fc4dfb5e6fd5b24a8d6b683f48d81422c6d399c5738d862ea9d224a14b3193')"></div>
        </div>

      <div class="visible-xs">My Profile</div>
</a>  </div>
</li>


  </ul>
</div>


    <main>
        <div id="layout-bars">
          
          
          
          
          
        </div>

      <article class="">

        
<div class="project row">
  <div class="col-xs-12 col-md-10 col-lg-8 contains-images">

      <h1 class="gap">0x05. Python - Exceptions</h1>

  <div data-react-class="tags/Tags" data-react-props="{&quot;tags&quot;:[{&quot;id&quot;:19,&quot;value&quot;:&quot;Python&quot;,&quot;author_id&quot;:null,&quot;created_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;,&quot;updated_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;}]}" data-react-cache-id="tags/Tags-0"></div>

  <div data-react-class="projects/ProjectMetadata" data-react-props="{&quot;metadata&quot;:{&quot;author&quot;:&quot;Guillaume&quot;,&quot;weight&quot;:1,&quot;correction&quot;:{&quot;released&quot;:true,&quot;requires_auto_correction&quot;:true,&quot;requires_manual_correction&quot;:false},&quot;bpi&quot;:{&quot;current&quot;:false,&quot;in_second_deadline&quot;:false,&quot;starts_at&quot;:&quot;2023-03-27T06:00:00.000+03:00&quot;,&quot;ends_at&quot;:&quot;2023-03-28T06:00:00.000+03:00&quot;,&quot;second_deadline_at&quot;:&quot;2023-03-30T06:00:00.000+03:00&quot;}}}" data-react-cache-id="projects/ProjectMetadata-0"></div>

  <div class="sm-gap clean well">
  <h4>In a nutshell&hellip;</h4>
  <ul>


      <li>
        <strong>Auto QA review:</strong>
          84.0/84 mandatory
            &
            51.0/51 optional
      </li>
    <li>
      <strong>Altogether:</strong>
        &nbsp;<strong>200.0%</strong>
        <ul>
          <li>Mandatory: 100.0%</li>
            <li>Optional: 100.0%</li>
            <li>
              Calculation:&nbsp;
                  100.0%
                    + (100.0% * 100.0%)
              &nbsp;==&nbsp;<strong>200.0%</strong>
            </li>
        </ul>
    </li>
  </ul>
</div>




    


    <div id="project_id" style="display: none" data-project-id="245"></div>



      

      

      <div class="panel panel-default" id="project-description">
  <div class="panel-body">
    <h2>Resources</h2>

<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="/rltoken/Yj7sDOzmKwICSHr7WEAW3A" title="Errors and Exceptions" target="_blank">Errors and Exceptions</a> </li>
<li><a href="/rltoken/xASzXarhF1sBhzYkJ14LvQ" title="Learn to Program 11 Static &amp; Exception Handling" target="_blank">Learn to Program 11 Static &amp; Exception Handling</a> (<em>starting at minute 7</em>)</li>
</ul>

<h2>Learning Objectives</h2>

<p>At the end of this project, you are expected to be able to <a href="/rltoken/ER6JIfkhcpsfFWZNN_BBvg" title="explain to anyone" target="_blank">explain to anyone</a>, <strong>without the help of Google</strong>:</p>

<h3>General</h3>

<ul>
<li>Why Python programming is awesome </li>
<li>What&rsquo;s the difference between errors and exceptions</li>
<li>What are exceptions and how to use them</li>
<li>When do we need to use exceptions</li>
<li>How to correctly handle an exception</li>
<li>What&rsquo;s the purpose of catching exceptions</li>
<li>How to raise a builtin exception</li>
<li>When do we need to implement a clean-up action after an exception</li>
</ul>

<h3>Copyright - Plagiarism</h3>

<ul>
<li>You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.</li>
<li>You will not be able to meet the objectives of this or any following project by copying and pasting someone else&rsquo;s work. </li>
<li>You are not allowed to publish any content of this project.</li>
<li>Any form of plagiarism is strictly forbidden and will result in removal from the program.</li>
</ul>

<h2>Requirements</h2>

<h3>General</h3>

<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5)</li>
<li>All your files should end with a new line</li>
<li>The first line of all your files should be exactly <code>#!/usr/bin/python3</code></li>
<li>A <code>README.md</code> file, at the root of the folder of the project, is mandatory</li>
<li>Your code should use the pycodestyle (version <code>2.8.*</code>)</li>
<li>All your files must be executable</li>
<li>The length of your files will be tested using <code>wc</code></li>
</ul>

  </div>
</div>


      

      

        
          <h2 class="gap">Tasks</h2>

    <div data-role="task1154" data-position="1" id="task-num-0">
      <div class="panel panel-default task-card " id="task-1154">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      0. Safe list printing
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1154" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write a function that prints <code>x</code> elements of a list.</p>

<ul>
<li>Prototype: <code>def safe_print_list(my_list=[], x=0):</code></li>
<li><code>my_list</code> can contain any type (integer, string, etc.)</li>
<li>All elements must be printed on the same line followed by a new line.</li>
<li><code>x</code> represents the number of elements to print</li>
<li><code>x</code> can be bigger than the length of <code>my_list</code></li>
<li>Returns the real number of elements printed</li>
<li>You have to use <code>try: / except:</code> </li>
<li>You are not allowed to import any module</li>
<li>You are not allowed to use <code>len()</code></li>
</ul>

<pre><code>guillaume@ubuntu:~/0x05$ cat 0-main.py
#!/usr/bin/python3
safe_print_list = __import__(&#39;0-safe_print_list&#39;).safe_print_list

my_list = [1, 2, 3, 4, 5]

nb_print = safe_print_list(my_list, 2)
print(&quot;nb_print: {:d}&quot;.format(nb_print))
nb_print = safe_print_list(my_list, len(my_list))
print(&quot;nb_print: {:d}&quot;.format(nb_print))
nb_print = safe_print_list(my_list, len(my_list) + 2)
print(&quot;nb_print: {:d}&quot;.format(nb_print))

guillaume@ubuntu:~/0x05$ ./0-main.py
12
nb_print: 2
12345
nb_print: 5
12345
nb_print: 5
guillaume@ubuntu:~/0x05$ 
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>0-safe_print_list.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1154">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1154" data-batch-id="62" data-toggle="modal" data-target="#task-1154-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1154-users-done-modal" data-task-id="1154" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "0. Safe list printing"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1154-modal-button" data-task-id="1154" data-toggle="modal" data-target="#task-test-correction-1154-correction-modal" id="task-num-0-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1154}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1154-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "0. Safe list printing"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1154" data-last-request-id="74831771">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1154">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1154">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1154}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1154" data-toggle="modal" data-target="#task-qa-review-1154-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1154}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1154-modal" data-correction-id="13408025" data-task-id="1154">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">0. Safe list printing</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1155" data-position="2" id="task-num-1">
      <div class="panel panel-default task-card " id="task-1155">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      1. Safe printing of an integers list
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1155" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write a function that prints an integer with <code>&quot;{:d}&quot;.format()</code>.</p>

<ul>
<li>Prototype: <code>def safe_print_integer(value):</code></li>
<li><code>value</code> can be any type (integer, string, etc.)</li>
<li>The integer should be printed followed by a new line</li>
<li>Returns <code>True</code> if <code>value</code> has been correctly printed (it means the <code>value</code> is an integer)</li>
<li>Otherwise, returns <code>False</code></li>
<li>You have to use <code>try: / except:</code> </li>
<li>You have to use <code>&quot;{:d}&quot;.format()</code> to print as integer</li>
<li>You are not allowed to import any module</li>
<li>You are not allowed to use <code>type()</code></li>
</ul>

<pre><code>guillaume@ubuntu:~/0x05$ cat 1-main.py
#!/usr/bin/python3
safe_print_integer = __import__(&#39;1-safe_print_integer&#39;).safe_print_integer

value = 89
has_been_print = safe_print_integer(value)
if not has_been_print:
    print(&quot;{} is not an integer&quot;.format(value))

value = -89
has_been_print = safe_print_integer(value)
if not has_been_print:
    print(&quot;{} is not an integer&quot;.format(value))

value = &quot;School&quot;
has_been_print = safe_print_integer(value)
if not has_been_print:
    print(&quot;{} is not an integer&quot;.format(value))

guillaume@ubuntu:~/0x05$ ./1-main.py
89
-89
School is not an integer
guillaume@ubuntu:~/0x05$ 
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>1-safe_print_integer.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1155">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1155" data-batch-id="62" data-toggle="modal" data-target="#task-1155-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1155-users-done-modal" data-task-id="1155" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "1. Safe printing of an integers list"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1155-modal-button" data-task-id="1155" data-toggle="modal" data-target="#task-test-correction-1155-correction-modal" id="task-num-1-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1155}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1155-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "1. Safe printing of an integers list"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1155" data-last-request-id="74831861">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1155">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1155">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1155}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1155" data-toggle="modal" data-target="#task-qa-review-1155-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1155}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1155-modal" data-correction-id="13408025" data-task-id="1155">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">1. Safe printing of an integers list</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1156" data-position="3" id="task-num-2">
      <div class="panel panel-default task-card " id="task-1156">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      2. Print and count integers
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1156" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write a function that prints the first <code>x</code> elements of a list and only integers.</p>

<ul>
<li>Prototype: <code>def safe_print_list_integers(my_list=[], x=0):</code></li>
<li><code>my_list</code> can contain any type (integer, string, etc.)</li>
<li>All integers have to be printed on the same line followed by a new line - other type of value in the list must be skipped (in silence).</li>
<li><code>x</code> represents the number of elements to access in <code>my_list</code></li>
<li><code>x</code> can be bigger than the length of <code>my_list</code> - if it&rsquo;s the case, an exception is expected to occur</li>
<li>Returns the real number of integers printed</li>
<li>You have to use <code>try: / except:</code> </li>
<li>You have to use <code>&quot;{:d}&quot;.format()</code> to print an integer</li>
<li>You are not allowed to import any module</li>
<li>You are not allowed to use <code>len()</code></li>
</ul>

<pre><code>guillaume@ubuntu:~/0x05$ cat 2-main.py
#!/usr/bin/python3
safe_print_list_integers = \
    __import__(&#39;2-safe_print_list_integers&#39;).safe_print_list_integers

my_list = [1, 2, 3, 4, 5]

nb_print = safe_print_list_integers(my_list, 2)
print(&quot;nb_print: {:d}&quot;.format(nb_print))

my_list = [1, 2, 3, &quot;School&quot;, 4, 5, [1, 2, 3]]
nb_print = safe_print_list_integers(my_list, len(my_list))
print(&quot;nb_print: {:d}&quot;.format(nb_print))

nb_print = safe_print_list_integers(my_list, len(my_list) + 2)
print(&quot;nb_print: {:d}&quot;.format(nb_print))

guillaume@ubuntu:~/0x05$ ./2-main.py
12
nb_print: 2
12345
nb_print: 5
12345Traceback (most recent call last):
  File &quot;./2-main.py&quot;, line 14, in &lt;module&gt;
    nb_print = safe_print_list_integers(my_list, len(my_list) + 2)
  File &quot;/0x05/2-safe_print_list_integers.py&quot;, line 7, in safe_print_list_integers
    print(&quot;{:d}&quot;.format(my_list[i]), end=&quot;&quot;)
IndexError: list index out of range
guillaume@ubuntu:~/0x05$ 
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>2-safe_print_list_integers.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1156">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1156" data-batch-id="62" data-toggle="modal" data-target="#task-1156-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1156-users-done-modal" data-task-id="1156" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "2. Print and count integers"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1156-modal-button" data-task-id="1156" data-toggle="modal" data-target="#task-test-correction-1156-correction-modal" id="task-num-2-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1156}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1156-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "2. Print and count integers"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1156" data-last-request-id="74831936">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1156">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1156">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1156}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1156" data-toggle="modal" data-target="#task-qa-review-1156-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1156}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1156-modal" data-correction-id="13408025" data-task-id="1156">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">2. Print and count integers</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1157" data-position="4" id="task-num-3">
      <div class="panel panel-default task-card " id="task-1157">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      3. Integers division with debug
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1157" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write a function that divides 2 integers and prints the result.</p>

<ul>
<li>Prototype: <code>def safe_print_division(a, b):</code></li>
<li>You can assume that <code>a</code> and <code>b</code> are integers</li>
<li>The result of the division should print on the <code>finally:</code> section preceded by <code>Inside result:</code></li>
<li>Returns the value of the division, otherwise: <code>None</code></li>
<li>You have to use <code>try: / except: / finally:</code> </li>
<li>You have to use <code>&quot;{}&quot;.format()</code> to print the result</li>
<li>You are not allowed to import any module</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x05$ cat 3-main.py
#!/usr/bin/python3
safe_print_division = __import__(&#39;3-safe_print_division&#39;).safe_print_division

a = 12
b = 2
result = safe_print_division(a, b)
print(&quot;{:d} / {:d} = {}&quot;.format(a, b, result))

a = 12
b = 0
result = safe_print_division(a, b)
print(&quot;{:d} / {:d} = {}&quot;.format(a, b, result))

guillaume@ubuntu:~/0x05$ ./3-main.py
Inside result: 6.0
12 / 2 = 6.0
Inside result: None
12 / 0 = None
guillaume@ubuntu:~/0x05$ 
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>3-safe_print_division.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1157">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1157" data-batch-id="62" data-toggle="modal" data-target="#task-1157-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1157-users-done-modal" data-task-id="1157" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "3. Integers division with debug"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1157-modal-button" data-task-id="1157" data-toggle="modal" data-target="#task-test-correction-1157-correction-modal" id="task-num-3-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1157}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1157-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "3. Integers division with debug"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1157" data-last-request-id="74832102">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1157">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1157">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1157}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1157" data-toggle="modal" data-target="#task-qa-review-1157-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1157}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1157-modal" data-correction-id="13408025" data-task-id="1157">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">3. Integers division with debug</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1158" data-position="5" id="task-num-4">
      <div class="panel panel-default task-card " id="task-1158">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      4. Divide a list
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1158" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write a function that divides element by element 2 lists.</p>

<ul>
<li>Prototype: <code>def list_division(my_list_1, my_list_2, list_length):</code></li>
<li><code>my_list_1</code> and <code>my_list_2</code> can contain any type (integer, string, etc.)</li>
<li><code>list_length</code> can be bigger than the length of both lists</li>
<li>Returns a new list (length = <code>list_length</code>) with all divisions</li>
<li>If 2 elements can&rsquo;t be divided, the division result should be equal to <code>0</code></li>
<li>If an element is not an integer or float:

<ul>
<li>print: <code>wrong type</code></li>
</ul></li>
<li>If the division can&rsquo;t be done (<code>/0</code>):

<ul>
<li>print: <code>division by 0</code></li>
</ul></li>
<li>If <code>my_list_1</code> or <code>my_list_2</code> is too short

<ul>
<li>print: <code>out of range</code></li>
</ul></li>
<li>You have to use <code>try: / except: / finally:</code> </li>
<li>You are not allowed to import any module</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x05$ cat 4-main.py
#!/usr/bin/python3
list_division = __import__(&#39;4-list_division&#39;).list_division

my_l_1 = [10, 8, 4]
my_l_2 = [2, 4, 4]
result = list_division(my_l_1, my_l_2, max(len(my_l_1), len(my_l_2)))
print(result)

print(&quot;--&quot;)

my_l_1 = [10, 8, 4, 4]
my_l_2 = [2, 0, &quot;H&quot;, 2, 7]
result = list_division(my_l_1, my_l_2, max(len(my_l_1), len(my_l_2)))
print(result)

guillaume@ubuntu:~/0x05$ ./4-main.py
[5.0, 2.0, 1.0]
--
division by 0
wrong type
out of range
[5.0, 0, 0, 2.0, 0]
guillaume@ubuntu:~/0x05$ 
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>4-list_division.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1158">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1158" data-batch-id="62" data-toggle="modal" data-target="#task-1158-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1158-users-done-modal" data-task-id="1158" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "4. Divide a list"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1158-modal-button" data-task-id="1158" data-toggle="modal" data-target="#task-test-correction-1158-correction-modal" id="task-num-4-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1158}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1158-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "4. Divide a list"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1158" data-last-request-id="74832240">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1158">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1158">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1158}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1158" data-toggle="modal" data-target="#task-qa-review-1158-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1158}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1158-modal" data-correction-id="13408025" data-task-id="1158">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">4. Divide a list</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1159" data-position="6" id="task-num-5">
      <div class="panel panel-default task-card " id="task-1159">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      5. Raise exception
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1159" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write a function that raises a type exception.</p>

<ul>
<li>Prototype: <code>def raise_exception():</code></li>
<li>You are not allowed to import any module</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x05$ cat 5-main.py
#!/usr/bin/python3
raise_exception = __import__(&#39;5-raise_exception&#39;).raise_exception

try:
    raise_exception()
except TypeError as te:
    print(&quot;Exception raised&quot;)

guillaume@ubuntu:~/0x05$ ./5-main.py
Exception raised
guillaume@ubuntu:~/0x05$ 
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>5-raise_exception.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1159">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1159" data-batch-id="62" data-toggle="modal" data-target="#task-1159-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1159-users-done-modal" data-task-id="1159" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "5. Raise exception"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1159-modal-button" data-task-id="1159" data-toggle="modal" data-target="#task-test-correction-1159-correction-modal" id="task-num-5-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1159}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1159-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "5. Raise exception"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1159" data-last-request-id="74832291">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1159">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1159">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1159}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1159" data-toggle="modal" data-target="#task-qa-review-1159-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1159}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1159-modal" data-correction-id="13408025" data-task-id="1159">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">5. Raise exception</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1160" data-position="7" id="task-num-6">
      <div class="panel panel-default task-card " id="task-1160">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      6. Raise a message
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1160" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write a function that raises a name exception with a message.</p>

<ul>
<li>Prototype: <code>def raise_exception_msg(message=&quot;&quot;):</code></li>
<li>You are not allowed to import any module</li>
</ul>

<pre><code>guillaume@ubuntu:~/0x05$ cat 6-main.py
#!/usr/bin/python3
raise_exception_msg = __import__(&#39;6-raise_exception_msg&#39;).raise_exception_msg

try:
    raise_exception_msg(&quot;C is fun&quot;)
except NameError as ne:
    print(ne)

guillaume@ubuntu:~/0x05$ ./6-main.py
C is fun
guillaume@ubuntu:~/0x05$ 
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>6-raise_exception_msg.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1160">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1160" data-batch-id="62" data-toggle="modal" data-target="#task-1160-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1160-users-done-modal" data-task-id="1160" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "6. Raise a message"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1160-modal-button" data-task-id="1160" data-toggle="modal" data-target="#task-test-correction-1160-correction-modal" id="task-num-6-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1160}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1160-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "6. Raise a message"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1160" data-last-request-id="74832336">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1160">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1160">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1160}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1160" data-toggle="modal" data-target="#task-qa-review-1160-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1160}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1160-modal" data-correction-id="13408025" data-task-id="1160">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">6. Raise a message</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1161" data-position="100" id="task-num-7">
      <div class="panel panel-default task-card " id="task-1161">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      7. Safe integer print with error message
    </h3>

    <div>
        <span class="label label-info">
          #advanced
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1161" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write a function that prints an integer.</p>

<ul>
<li>Prototype: <code>def safe_print_integer_err(value):</code></li>
<li><code>value</code> can be any type (integer, string, etc.)</li>
<li>The integer should be printed followed by a new line</li>
<li>Returns <code>True</code> if <code>value</code> has been correctly printed (it means the <code>value</code> is an integer)</li>
<li>Otherwise, returns <code>False</code> and prints in <code>stderr</code> the error precede by <code>Exception:</code></li>
<li>You have to use <code>try: / except:</code> </li>
<li>You have to use <code>&quot;{:d}&quot;.format()</code> to print as integer</li>
<li>You are not allowed to use <code>type()</code></li>
</ul>

<pre><code>guillaume@ubuntu:~/0x05$ cat 100-main.py
#!/usr/bin/python3
safe_print_integer_err = \
    __import__(&#39;100-safe_print_integer_err&#39;).safe_print_integer_err

value = 89
has_been_print = safe_print_integer_err(value)
if not has_been_print:
    print(&quot;{} is not an integer&quot;.format(value))

value = -89
has_been_print = safe_print_integer_err(value)
if not has_been_print:
    print(&quot;{} is not an integer&quot;.format(value))

value = &quot;School&quot;
has_been_print = safe_print_integer_err(value)
if not has_been_print:
    print(&quot;{} is not an integer&quot;.format(value))

guillaume@ubuntu:~/0x05$ ./100-main.py
89
-89
Exception: Unknown format code &#39;d&#39; for object of type &#39;str&#39;
School is not an integer
guillaume@ubuntu:~/0x05$ ./100-main.py 2&gt; /dev/null
89
-89
School is not an integer
guillaume@ubuntu:~/0x05$ 
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>100-safe_print_integer_err.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1161">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1161" data-batch-id="62" data-toggle="modal" data-target="#task-1161-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1161-users-done-modal" data-task-id="1161" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "7. Safe integer print with error message"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1161-modal-button" data-task-id="1161" data-toggle="modal" data-target="#task-test-correction-1161-correction-modal" id="task-num-7-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1161}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1161-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "7. Safe integer print with error message"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1161" data-last-request-id="74832383">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1161">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1161">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1161}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1161" data-toggle="modal" data-target="#task-qa-review-1161-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1161}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1161-modal" data-correction-id="13408025" data-task-id="1161">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">7. Safe integer print with error message</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1162" data-position="101" id="task-num-8">
      <div class="panel panel-default task-card " id="task-1162">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      8. Safe function
    </h3>

    <div>
        <span class="label label-info">
          #advanced
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1162" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write a function that executes a function safely.  </p>

<ul>
<li>Prototype: <code>def safe_function(fct, *args):</code></li>
<li>You can assume <code>fct</code> will be always a pointer to a function</li>
<li>Returns the result of the function,</li>
<li>Otherwise, returns <code>None</code> if something happens during the function and prints in <code>stderr</code> the error precede by <code>Exception:</code></li>
<li>You have to use <code>try: / except:</code> </li>
</ul>

<pre><code>guillaume@ubuntu:~/0x05$ cat 101-main.py
#!/usr/bin/python3
safe_function = __import__(&#39;101-safe_function&#39;).safe_function


def my_div(a, b):
    return a / b

result = safe_function(my_div, 10, 2)
print(&quot;result of my_div: {}&quot;.format(result))

result = safe_function(my_div, 10, 0)
print(&quot;result of my_div: {}&quot;.format(result))


def print_list(my_list, len):
    i = 0
    while i &lt; len:
        print(my_list[i])
        i += 1
    return len

result = safe_function(print_list, [1, 2, 3, 4], 10)
print(&quot;result of print_list: {}&quot;.format(result))

guillaume@ubuntu:~/0x05$ ./101-main.py
result of my_div: 5.0
Exception: division by zero
result of my_div: None
1
2
3
4
Exception: list index out of range
result of print_list: None
guillaume@ubuntu:~/0x05$ ./101-main.py 2&gt; /dev/null
result of my_div: 5.0
result of my_div: None
1
2
3
4
result of print_list: None
guillaume@ubuntu:~/0x05$ 
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>101-safe_function.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1162">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1162" data-batch-id="62" data-toggle="modal" data-target="#task-1162-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1162-users-done-modal" data-task-id="1162" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "8. Safe function"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1162-modal-button" data-task-id="1162" data-toggle="modal" data-target="#task-test-correction-1162-correction-modal" id="task-num-8-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1162}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1162-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "8. Safe function"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1162" data-last-request-id="74832497">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1162">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1162">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1162}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1162" data-toggle="modal" data-target="#task-qa-review-1162-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1162}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1162-modal" data-correction-id="13408025" data-task-id="1162">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">8. Safe function</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1163" data-position="102" id="task-num-9">
      <div class="panel panel-default task-card " id="task-1163">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      9. ByteCode -&gt; Python #4
    </h3>

    <div>
        <span class="label label-info">
          #advanced
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1163" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Write the Python function <code>def magic_calculation(a, b):</code> that does exactly the same as the following Python bytecode:</p>

<pre><code>  3           0 LOAD_CONST               1 (0)
              3 STORE_FAST               2 (result)

  4           6 SETUP_LOOP              94 (to 103)
              9 LOAD_GLOBAL              0 (range)
             12 LOAD_CONST               2 (1)
             15 LOAD_CONST               3 (3)
             18 CALL_FUNCTION            2 (2 positional, 0 keyword pair)
             21 GET_ITER
        &gt;&gt;   22 FOR_ITER                77 (to 102)
             25 STORE_FAST               3 (i)

  5          28 SETUP_EXCEPT            49 (to 80)

  6          31 LOAD_FAST                3 (i)
             34 LOAD_FAST                0 (a)
             37 COMPARE_OP               4 (&gt;)
             40 POP_JUMP_IF_FALSE       58

  7          43 LOAD_GLOBAL              1 (Exception)
             46 LOAD_CONST               4 (&#39;Too far&#39;)
             49 CALL_FUNCTION            1 (1 positional, 0 keyword pair)
             52 RAISE_VARARGS            1
             55 JUMP_FORWARD            18 (to 76)

  9     &gt;&gt;   58 LOAD_FAST                2 (result)
             61 LOAD_FAST                0 (a)
             64 LOAD_FAST                1 (b)
             67 BINARY_POWER
             68 LOAD_FAST                3 (i)
             71 BINARY_TRUE_DIVIDE
             72 INPLACE_ADD
             73 STORE_FAST               2 (result)
        &gt;&gt;   76 POP_BLOCK
             77 JUMP_ABSOLUTE           22

 10     &gt;&gt;   80 POP_TOP
             81 POP_TOP
             82 POP_TOP

 11          83 LOAD_FAST                1 (b)
             86 LOAD_FAST                0 (a)
             89 BINARY_ADD
             90 STORE_FAST               2 (result)

 12          93 BREAK_LOOP
             94 POP_EXCEPT
             95 JUMP_ABSOLUTE           22
             98 END_FINALLY
             99 JUMP_ABSOLUTE           22
        &gt;&gt;  102 POP_BLOCK

 13     &gt;&gt;  103 LOAD_FAST                2 (result)
            106 RETURN_VALUE
</code></pre>

<ul>
<li>Tip: <a href="/rltoken/-eivu0w172OUPm-iCeKgtw" title="Python bytecode" target="_blank">Python bytecode</a></li>
</ul>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>102-magic_calculation.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1163">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1163" data-batch-id="62" data-toggle="modal" data-target="#task-1163-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1163-users-done-modal" data-task-id="1163" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "9. ByteCode -&gt; Python #4"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1163-modal-button" data-task-id="1163" data-toggle="modal" data-target="#task-test-correction-1163-correction-modal" id="task-num-9-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1163}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1163-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "9. ByteCode -&gt; Python #4"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1163" data-last-request-id="74832541">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1163">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1163">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1163}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1163" data-toggle="modal" data-target="#task-qa-review-1163-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1163}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1163-modal" data-correction-id="13408025" data-task-id="1163">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">9. ByteCode -&gt; Python #4</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task1164" data-position="103" id="task-num-10">
      <div class="panel panel-default task-card " id="task-1164">
  <span id="user_id" data-id="205867"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      10. CPython #2: PyFloatObject
    </h3>

    <div>
        <span class="label label-info">
          #advanced
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="205867"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="1164" data-correction-id="13408025">
        <div class="task_progress_bar" style="width: 100.0%">
          <div class="task_score_bar" style="width: 100.0%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">100.0%</span> (<span class="task_progress_value">Checks completed: 100.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Create three C functions that print some basic info about Python lists, Python bytes an Python float objects.<br />
<br />
<img src="https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/070710952984e4d126e114405cefe83af2271ce8.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230420%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230420T192654Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b294c3cdc337c627aecd860c7bc08040fe9fc99a9b31291284a0d3b5f52ce6e6" alt="" loading='lazy' style="" />
<br />
Python lists:</p>

<ul>
<li>Prototype: <code>void print_python_list(PyObject *p);</code></li>
<li>Format: see example</li>
<li>If <code>p</code> is not a valid <code>PyListObject</code>, print an error message (see example)</li>
</ul>

<p>Python bytes:</p>

<ul>
<li>Prototype: <code>void print_python_bytes(PyObject *p);</code></li>
<li>Format: see example</li>
<li>Line &ldquo;first X bytes&rdquo;: print a maximum of 10 bytes</li>
<li>If <code>p</code> is not a valid <code>PyBytesObject</code>, print an error message (see example)</li>
</ul>

<p>Python float:</p>

<ul>
<li>Prototype: <code>void print_python_float(PyObject *p);</code></li>
<li>Format: see example</li>
<li>If <code>p</code> is not a valid <code>PyFloatObject</code>, print an error message (see example)</li>
<li>Read <code>/usr/include/python3.4/floatobject.h</code></li>
</ul>

<p>About:</p>

<ul>
<li>Python version: 3.4</li>
<li>You are allowed to use the C standard library</li>
<li>Your shared library will be compiled with this command line: <code>gcc -Wall -Werror -Wextra -pedantic -std=c99 -shared -Wl,-soname,libPython.so -o libPython.so -fPIC -I/usr/include/python3.4 103-python.c</code></li>
<li>You are not allowed to use the following macros/functions:

<ul>
<li><code>Py_SIZE</code></li>
<li><code>Py_TYPE</code></li>
<li><code>PyList_Size</code></li>
<li><code>PyList_GetItem</code></li>
<li><code>PyBytes_AS_STRING</code></li>
<li><code>PyBytes_GET_SIZE</code></li>
<li><code>PyBytes_AsString</code></li>
<li><code>PyBytes_AsStringAndSize</code></li>
<li><code>PyFloat_AS_DOUBLE</code></li>
<li><code>PySequence_GetItem</code></li>
<li><code>PySequence_Fast_GET_SIZE</code></li>
<li><code>PySequence_Fast_GET_ITEM</code></li>
<li><code>PySequence_ITEM</code></li>
<li><code>PySequence_Fast_ITEMS</code></li>
</ul></li>
</ul>

<p><strong>NOTE</strong>:</p>

<ul>
<li>The python script will be launched using the <code>-u</code> option (Force <code>stdout</code> to be unbuffered).</li>
<li>It is <strong>strongly</strong> advised to either use <code>setbuf(stdout, NULL);</code> or <code>fflush(stdout)</code> in your C functions IF you choose to use <code>printf</code>. The reason to that is that Python<code>s</code>print<code>and libC</code>s <code>printf</code> don&rsquo;t share the same buffer, and the output can appear disordered.</li>
</ul>

<pre><code>julien@ubuntu:~/CPython$ python3 --version
Python 3.4.3
julien@ubuntu:~/CPython$ gcc -Wall -Werror -Wextra -pedantic -std=c99 -shared -Wl,-soname,libPython.so -o libPython.so -fPIC -I/usr/include/python3.4 103-python.c
julien@ubuntu:~/CPython$ cat 103-tests.py 
#!/usr/bin/python3 -u

import ctypes

lib = ctypes.CDLL(&#39;./libPython.so&#39;)
lib.print_python_list.argtypes = [ctypes.py_object]
lib.print_python_bytes.argtypes = [ctypes.py_object]
lib.print_python_float.argtypes = [ctypes.py_object]
s = b&quot;Hello&quot;
lib.print_python_bytes(s);
b = b&#39;\xff\xf8\x00\x00\x00\x00\x00\x00&#39;;
lib.print_python_bytes(b);
b = b&#39;What does the \&#39;b\&#39; character do in front of a string literal?&#39;;
lib.print_python_bytes(b);
l = [b&#39;Hello&#39;, b&#39;World&#39;]
lib.print_python_list(l)
del l[1]
lib.print_python_list(l)
l = l + [4, 5, 6.0, (9, 8), [9, 8, 1024], b&quot;School&quot;, &quot;Betty&quot;]
lib.print_python_list(l)
l = []
lib.print_python_list(l)
l.append(0)
lib.print_python_list(l)
l.append(1)
l.append(2)
l.append(3)
l.append(4)
lib.print_python_list(l)
l.pop()
lib.print_python_list(l)
l = [&quot;School&quot;]
lib.print_python_list(l)
lib.print_python_bytes(l);
f = 3.14
lib.print_python_float(f);
l = [-1.0, -0.1, 0.0, 1.0, 3.14, 3.14159, 3.14159265, 3.141592653589793238462643383279502884197169399375105820974944592307816406286]
print(l)
lib.print_python_list(l);
lib.print_python_float(l);
lib.print_python_list(f);
julien@ubuntu:~/CPython$ ./103-tests.py 
[.] bytes object info
  size: 5
  trying string: Hello
  first 6 bytes: 48 65 6c 6c 6f 00
[.] bytes object info
  size: 8
  trying string: ??
  first 9 bytes: ff f8 00 00 00 00 00 00 00
[.] bytes object info
  size: 60
  trying string: What does the &#39;b&#39; character do in front of a string literal?
  first 10 bytes: 57 68 61 74 20 64 6f 65 73 20
[*] Python list info
[*] Size of the Python List = 2
[*] Allocated = 2
Element 0: bytes
[.] bytes object info
  size: 5
  trying string: Hello
  first 6 bytes: 48 65 6c 6c 6f 00
Element 1: bytes
[.] bytes object info
  size: 5
  trying string: World
  first 6 bytes: 57 6f 72 6c 64 00
[*] Python list info
[*] Size of the Python List = 1
[*] Allocated = 2
Element 0: bytes
[.] bytes object info
  size: 5
  trying string: Hello
  first 6 bytes: 48 65 6c 6c 6f 00
[*] Python list info
[*] Size of the Python List = 8
[*] Allocated = 8
Element 0: bytes
[.] bytes object info
  size: 5
  trying string: Hello
  first 6 bytes: 48 65 6c 6c 6f 00
Element 1: int
Element 2: int
Element 3: float
[.] float object info
  value: 6.0
Element 4: tuple
Element 5: list
Element 6: bytes
[.] bytes object info
  size: 9
  trying string: School
  first 10 bytes: 48 6f 6c 62 65 72 74 6f 6e 00
Element 7: str
[*] Python list info
[*] Size of the Python List = 0
[*] Allocated = 0
[*] Python list info
[*] Size of the Python List = 1
[*] Allocated = 4
Element 0: int
[*] Python list info
[*] Size of the Python List = 5
[*] Allocated = 8
Element 0: int
Element 1: int
Element 2: int
Element 3: int
Element 4: int
[*] Python list info
[*] Size of the Python List = 4
[*] Allocated = 8
Element 0: int
Element 1: int
Element 2: int
Element 3: int
[*] Python list info
[*] Size of the Python List = 1
[*] Allocated = 1
Element 0: str
[.] bytes object info
  [ERROR] Invalid Bytes Object
[.] float object info
  value: 3.14
[-1.0, -0.1, 0.0, 1.0, 3.14, 3.14159, 3.14159265, 3.141592653589793]
[*] Python list info
[*] Size of the Python List = 8
[*] Allocated = 8
Element 0: float
[.] float object info
  value: -1.0
Element 1: float
[.] float object info
  value: -0.1
Element 2: float
[.] float object info
  value: 0.0
Element 3: float
[.] float object info
  value: 1.0
Element 4: float
[.] float object info
  value: 3.14
Element 5: float
[.] float object info
  value: 3.14159
Element 6: float
[.] float object info
  value: 3.14159265
Element 7: float
[.] float object info
  value: 3.141592653589793
[.] float object info
  [ERROR] Invalid Float Object
[*] Python list info
  [ERROR] Invalid List Object
julien@ubuntu:~/CPython$
</code></pre>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-higher_level_programming</code></li>
            <li>Directory: <code>0x05-python-exceptions</code></li>
            <li>File: <code>103-python.c</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm yes" data-task-id="1164">
      <span class="no"><i aria-hidden="true" class="fa fa-square-o "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa fa-check-square-o "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa fa-spinner  fa-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="1164" data-batch-id="62" data-toggle="modal" data-target="#task-1164-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-1164-users-done-modal" data-task-id="1164" data-batch-id="62">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Students who are done with "10. CPython #2: PyFloatObject"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-1164-modal-button" data-task-id="1164" data-toggle="modal" data-target="#task-test-correction-1164-correction-modal" id="task-num-10-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1164}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-1164-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "10. CPython #2: PyFloatObject"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="1164" data-last-request-id="74833815">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="1164">
        <i aria-hidden="true" class="fa fa-info-circle "></i>
    </button>
    <div class="help-container" data-task-id="1164">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa fa-check-circle "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa fa-times-circle "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>



    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:1164}"><i aria-hidden="true" class="fa fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="1164" data-toggle="modal" data-target="#task-qa-review-1164-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:1164}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-1164-modal" data-correction-id="13408025" data-task-id="1164">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">10. CPython #2: PyFloatObject</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>





          <div class="modal fade" id="container-specs-modal"><div class="modal-dialog modal-lg"><div class="modal-content"><div class="modal-header"><button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button><h4 class="modal-title">Recommended Sandboxes</h4></div><div class="modal-body"><div data-react-class="user_containers/ContainerSpecs" data-react-props="{&quot;containerModelName&quot;:&quot;Sandbox&quot;,&quot;containerSpecs&quot;:[{&quot;description&quot;:&quot;\u003cp\u003eUbuntu 14.04 with all tools needed and Python 3.4\u003c/p\u003e\n&quot;,&quot;id&quot;:5,&quot;name&quot;:&quot;Ubuntu 14.04 - Python 3.4&quot;,&quot;online&quot;:true},{&quot;description&quot;:&quot;\u003cp\u003eBasic Ubuntu 20.04, with vim, emacs, curl, wget and all needed for Foundations\u003c/p\u003e\n&quot;,&quot;id&quot;:39,&quot;name&quot;:&quot;Ubuntu 20.04&quot;,&quot;online&quot;:true,&quot;container&quot;:{&quot;container_id&quot;:&quot;28f0705dcf62fc351ae33ed3c590891ed8257916db846dde9fb62e73faf0c4d3&quot;,&quot;id&quot;:224694,&quot;restart_uri&quot;:&quot;/user_containers/224694/restart.json&quot;,&quot;status&quot;:&quot;running&quot;,&quot;uri&quot;:&quot;/user_containers/224694.json&quot;,&quot;wake_uri&quot;:&quot;/user_containers/224694/wake.json&quot;,&quot;webterm_uri&quot;:&quot;/user_containers/224694/webterm&quot;,&quot;host&quot;:&quot;28f0705dcf62.b20b5966.alx-cod.online&quot;,&quot;password&quot;:&quot;bbd604c1866ae8fc893c&quot;,&quot;ports&quot;:{&quot;3000&quot;:56220,&quot;4000&quot;:56218,&quot;443&quot;:56221,&quot;5000&quot;:56217,&quot;5001&quot;:56216,&quot;80&quot;:56222,&quot;8080&quot;:56214,&quot;22&quot;:56223,&quot;8000&quot;:56215,&quot;3306&quot;:56219}}}],&quot;containersLimit&quot;:2,&quot;csrfToken&quot;:&quot;m5dv6RBR5gUy69SyXpZe_fiuAtK1DvMEEUGb1Ci2yHmwoexbsefKakQvIA7acvbhUmm_qsqqfj1f1f6mLrs9vQ&quot;,&quot;startStatusURI&quot;:&quot;/user_containers/start_status.json&quot;,&quot;startURI&quot;:&quot;/user_containers/start.json&quot;}" data-react-cache-id="user_containers/ContainerSpecs-0"></div></div></div></div></div>

  </div>
</div>


      </article>

      <div class="copyright">Copyright © 2023 ALX, All rights reserved.</div>

    </main>

        <button class="btn btn-primary" id="search-button" data-search-active="false" data-toggle="modal" data-target="#search-modal">
  <i aria-hidden="true" class="fa fa-search "></i>
  <i aria-hidden="true" class="fa fa-window-minimize "></i>
</button>

        <div class="modal fade" id="search-modal" tabindex="-1" role="dialog" aria-labelledby="search-modal-label">
    <div class="modal-dialog modal-md">
        <div class="modal-content">
            <div class="modal-header">
                <div id="search-bar-container">
    <input id="search-bar"
            type="text"
            name="hbtn-search-bar"
            placeholder="✨Start search by typing in this field✨">
</div>

            </div>
            <div class="modal-body">
                <div id="modal-spinner" class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div id="search-results-container">
</div>

            </div>
        </div>
    </div>
</div>



        <div class="modal fade" id="markdownGuideModal" tabindex="-1" role="dialog" aria-labelledby="markdownGuideModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-md">
    <div class="modal-content">
        <div class="modal-header">
          <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
          <h4 class="modal-title">Markdown Guide</h4>
        </div>
        <div class="modal-body">
            <h4>Emphasis</h4>
<pre>**<strong>bold</strong>**
*<em>italics</em>*
~~<strike>strikethrough</strike>~~</pre>
<h4>Headers</h4>
<pre># Big header
## Medium header
### Small header
#### Tiny header</pre>
<h4>Lists</h4>
<pre>* Generic list item
* Generic list item
* Generic list item

1. Numbered list item
2. Numbered list item
3. Numbered list item</pre>
<h4>Links</h4>
<pre>[Text to display](http://www.example.com)</pre>
<h4>Quotes</h4>
<pre>> This is a quote.
> It can span multiple lines!</pre>
<h4>Images</h4>
<p>CSS style available: <code>width, height, opacity</code></p>
<pre>![](http://www.example.com/image.jpg)
![](http://www.example.com/image.jpg | width: 200px)
![](http://www.example.com/image.jpg | height: 124px | width: 80px | opacity: 0.6)
</pre>
<h4>Tables</h4>
<pre>| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| John     | Doe      | Male     |
| Mary     | Smith    | Female   |

<em>Or without aligning the columns...</em>

| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| John | Doe | Male |
| Mary | Smith | Female |
</pre>
<h4>Displaying code</h4>
<pre>`var example = "hello!";`

<em>Or spanning multiple lines...</em>

```
var example = "hello!";
alert(example);
```</pre>
        </div>
    </div>
  </div>
</div>


  </body>
</html>

