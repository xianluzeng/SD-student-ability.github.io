<!DOCTYPE html>

<html lang="zh-CN">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>学生能力维度分析系统</title>

    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/0.4.1/html2canvas.min.js"></script>

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

    <style>

        body {

            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

            background-color: #f0f2f5;

            color: #212529;

            padding-top: 20px;

        }

        .header {

            background: linear-gradient(135deg, #4361ee, #3f37c9);

            color: white;

            padding: 30px 0;

            margin-bottom: 30px;

            box-shadow: 0 8px 16px rgba(0,0,0,0.1);

        }

        .card {

            margin-bottom: 25px;

            transition: transform 0.3s;

        }

        .card:hover {

            transform: translateY(-8px);

            box-shadow: 0 12px 20px rgba(0,0,0,0.12);

        }

        .btn-primary {

            background: linear-gradient(135deg, #4361ee, #3f37c9);

            border: none;

            padding: 12px 25px;

            font-weight: 600;

            border-radius: 10px;

        }

        .dimension-card {

            background-color: #f8f9fa;

            border-left: 5px solid #4361ee;

            padding: 18px;

            margin-bottom: 18px;

            border-radius: 10px;

        }

        .dimension-card:hover {

            background-color: #e9ecef;

        }

        .dimension-input {

            width: 100%;

            height: 10px;

            border-radius: 5px;

        }

        .chart-container {

            height: 400px;

            margin: 25px 0;

        }

        .floating-btn {

            position: fixed;

            bottom: 30px;

            right: 30px;

            width: 70px;

            height: 70px;

            border-radius: 50%;

            background: linear-gradient(135deg, #4361ee, #3f37c9);

            color: white;

            display: flex;

            align-items: center;

            justify-content: center;

            font-size: 2rem;

            box-shadow: 0 6px 15px rgba(67, 97, 238, 0.4);

            cursor: pointer;

        }

    </style>

</head>

<body>



    <div class="container">

        <!-- 页头 -->

        <div class="header text-center">

            <h1>学生能力维度分析系统</h1>

            <p class="lead">基于六个核心维度评估学生综合能力</p>

        </div>



        <!-- 添加学生信息 -->

        <div class="row">

            <div class="col-md-6">

                <div class="card">

                    <div class="card-header">学生能力评估</div>

                    <div class="card-body">

                        <div class="mb-4">

                            <label class="form-label">选择班级</label>

                            <select class="form-select" id="classSelect">

                                <option value="1">高一(1)班</option>

                                <option value="2">高一(2)班</option>

                                <option value="3">高一(3)班</option>

                            </select>

                        </div>

                        <div class="mb-4">

                            <label class="form-label">学生姓名</label>

                            <input type="text" class="form-control" id="studentName" placeholder="输入学生姓名">

                        </div>



                        <h5 class="mb-4">能力维度评分 (0-10分)</h5>



                        <!-- 维度评分 -->

                        <div class="mb-3">

                            <div class="dimension-card">

                                <div class="dimension-label">1. 知识探究与批判性思维</div>

                                <input type="range" class="form-range dimension-input" min="0" max="10" value="8">

                            </div>

                            <div class="dimension-card">

                                <div class="dimension-label">2. 创造性表达与艺术鉴赏</div>

                                <input type="range" class="form-range dimension-input" min="0" max="10" value="7">

                            </div>

                            <div class="dimension-card">

                                <div class="dimension-label">3. 协作与沟通能力</div>

                                <input type="range" class="form-range dimension-input" min="0" max="10" value="9">

                            </div>

                            <div class="dimension-card">

                                <div class="dimension-label">4. 逻辑推理与问题解决能力</div>

                                <input type="range" class="form-range dimension-input" min="0" max="10" value="7">

                            </div>

                            <div class="dimension-card">

                                <div class="dimension-label">5. 社会责任与全球视野</div>

                                <input type="range" class="form-range dimension-input" min="0" max="10" value="6">

                            </div>

                            <div class="dimension-card">

                                <div class="dimension-label">6. 自我反思与个人成长</div>

                                <input type="range" class="form-range dimension-input" min="0" max="10" value="8">

                            </div>

                        </div>



                        <button class="btn btn-primary" id="generateChartBtn">生成能力雷达图</button>

                    </div>

                </div>

            </div>



            <div class="col-md-6">

                <div class="card">

                    <div class="card-header">能力维度雷达图</div>

                    <div class="card-body">

                        <div class="chart-container">

                            <canvas id="radarChart"></canvas>

                        </div>

                        <button class="btn btn-primary" id="downloadBtn">下载图表</button>

                    </div>

                </div>

            </div>

        </div>



        <div class="floating-btn">

            <i class="fas fa-plus"></i>

        </div>



    </div>



    <script>

        // 初始化学生数据

        const students = [

            { id: 1, name: '张思睿', classId: 1, scores: [8, 7, 9, 7, 6, 8] },

            { id: 2, name: '李欣怡', classId: 2, scores: [9, 8, 7, 8, 6, 7] }

        ];



        // 生成雷达图

        function generateRadarChart(student) {

            const ctx = document.getElementById('radarChart').getContext('2d');

            const dimensions = ['知识探究与批判性思维', '创造性表达与艺术鉴赏', '协作与沟通能力', '逻辑推理与问题解决能力', '社会责任与全球视野', '自我反思与个人成长'];

            const radarChart = new Chart(ctx, {

                type: 'radar',

                data: {

                    labels: dimensions,

                    datasets: [{

                        label: student.name,

                        data: student.scores,

                        backgroundColor: 'rgba(67, 97, 238, 0.2)',

                        borderColor: 'rgba(67, 97, 238, 1)',

                        borderWidth: 3,

                        pointBackgroundColor: 'rgba(67, 97, 238, 1)',

                        pointRadius: 5

                    }]

                },

                options: {

                    scales: {

                        r: {

                            angleLines: { display: true, color: 'rgba(0, 0, 0, 0.1)' },

                            suggestedMin: 0,

                            suggestedMax: 10,

                            ticks: { stepSize: 2, backdropColor: 'transparent', color: '#6c757d' },

                            grid: { color: 'rgba(0, 0, 0, 0.05)' },

                            pointLabels: { font: { size: 12, weight: 'bold' }, padding: 15 }

                        }

                    },

                    plugins: { legend: { display: false }, tooltip: { backgroundColor: 'rgba(0, 0, 0, 0.8)', titleFont: { size: 14 }, bodyFont: { size: 13 }, padding: 12, displayColors: false } },

                    maintainAspectRatio: false,

                    responsive: true

                }

            });

        }



        // 下载图表功能

        document.getElementById('downloadBtn').addEventListener('click', function() {

            html2canvas(document.getElementById('radarChart')).then(canvas => {

                const link = document.createElement('a');

                link.href = canvas.toDataURL();

                link.download = 'student_radar_chart.png';

                link.click();

            });

        });



        // 生成雷达图按钮事件

        document.getElementById('generateChartBtn').addEventListener('click', function() {

            const studentName = document.getElementById('studentName').value;

            const classId = document.getElementById('classSelect').value;



            const student = students.find(s => s.name === studentName && s.classId === parseInt(classId));



            if (student) {

                generateRadarChart(student);

            } else {

                alert('没有找到该学生');

            }

        });

    </script>



</body>

</html>
