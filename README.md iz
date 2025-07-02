<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JobConnect Pro - Hiring Platform</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Custom CSS for elements that need more specific styling */
        .gradient-bg {
            background: linear-gradient(135deg, #3b82f6 0%, #8b5cf6 100%);
        }
        .job-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
        }
        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
        .sidebar {
            transition: all 0.3s ease;
        }
        @media (max-width: 768px) {
            .sidebar {
                transform: translateX(-100%);
                position: fixed;
                z-index: 50;
                top: 0;
                left: 0;
                height: 100vh;
            }
            .sidebar.open {
                transform: translateX(0);
            }
        }
        .progress-bar {
            transition: width 0.5s ease;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Navigation -->
    <nav class="gradient-bg text-white shadow-lg">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-4">
                <button id="mobile-menu-button" class="md:hidden focus:outline-none">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
                <a href="#" class="text-2xl font-bold flex items-center">
                    <i class="fas fa-handshake mr-2"></i>
                    <span>JobConnect Pro</span>
                </a>
            </div>
            <div class="hidden md:flex items-center space-x-6">
                <a href="#" class="hover:text-blue-200">Home</a>
                <a href="#jobs" class="hover:text-blue-200">Find Jobs</a>
                <a href="#employers" class="hover:text-blue-200">For Employers</a>
                <a href="#pricing" class="hover:text-blue-200">Pricing</a>
                <a href="#contact" class="hover:text-blue-200">Contact</a>
            </div>
            <div class="flex items-center space-x-4">
                <button id="login-btn" class="bg-white text-blue-600 px-4 py-2 rounded-lg font-medium hover:bg-blue-50 transition">
                    Login
                </button>
                <button class="hidden md:block bg-blue-800 text-white px-4 py-2 rounded-lg font-medium hover:bg-blue-900 transition">
                    Post a Job
                </button>
            </div>
        </div>
    </nav>

    <!-- Mobile Sidebar -->
    <div id="sidebar" class="sidebar bg-white w-64 shadow-lg md:hidden">
        <div class="p-4 border-b">
            <div class="flex justify-between items-center">
                <span class="text-xl font-bold">Menu</span>
                <button id="close-sidebar" class="focus:outline-none">
                    <i class="fas fa-times"></i>
                </button>
            </div>
        </div>
        <div class="p-4">
            <a href="#" class="block py-2 text-gray-700 hover:text-blue-600">Home</a>
            <a href="#jobs" class="block py-2 text-gray-700 hover:text-blue-600">Find Jobs</a>
            <a href="#employers" class="block py-2 text-gray-700 hover:text-blue-600">For Employers</a>
            <a href="#pricing" class="block py-2 text-gray-700 hover:text-blue-600">Pricing</a>
            <a href="#contact" class="block py-2 text-gray-700 hover:text-blue-600">Contact</a>
            <div class="mt-4 pt-4 border-t">
                <button class="w-full bg-blue-600 text-white px-4 py-2 rounded-lg font-medium hover:bg-blue-700 transition">
                    Post a Job
                </button>
            </div>
        </div>
    </div>

    <!-- Hero Section -->
    <section class="gradient-bg text-white py-16 md:py-24">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-10 md:mb-0">
                    <h1 class="text-4xl md:text-5xl font-bold mb-6">Connect Top Talent With Great Companies</h1>
                    <p class="text-xl mb-8">The most comprehensive hiring platform with automated job imports, video interviews, and advanced candidate tracking.</p>
                    <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                        <button class="bg-white text-blue-600 px-6 py-3 rounded-lg font-medium hover:bg-blue-50 transition">
                            Find Jobs <i class="fas fa-search ml-2"></i>
                        </button>
                        <button class="bg-blue-800 text-white px-6 py-3 rounded-lg font-medium hover:bg-blue-900 transition">
                            Post a Job <i class="fas fa-briefcase ml-2"></i>
                        </button>
                    </div>
                </div>
                <div class="md:w-1/2 flex justify-center">
                    <img src="https://images.unsplash.com/photo-1521791055366-0d553872125f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1350&q=80" alt="Hiring Platform" class="rounded-lg shadow-xl w-full max-w-md">
                </div>
            </div>
        </div>
    </section>

    <!-- Job Search Section -->
    <section id="jobs" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Find Your Dream Job</h2>
            
            <!-- Search Filters -->
            <div class="bg-gray-100 p-6 rounded-lg mb-8">
                <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
                    <div>
                        <label class="block text-gray-700 mb-2">Job Title</label>
                        <input type="text" placeholder="e.g. Software Engineer" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                    </div>
                    <div>
                        <label class="block text-gray-700 mb-2">Location</label>
                        <input type="text" placeholder="e.g. New York" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                    </div>
                    <div>
                        <label class="block text-gray-700 mb-2">Job Type</label>
                        <select class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                            <option>All Types</option>
                            <option>Full-time</option>
                            <option>Part-time</option>
                            <option>Contract</option>
                            <option>Remote</option>
                        </select>
                    </div>
                    <div class="flex items-end">
                        <button class="w-full bg-blue-600 text-white px-4 py-2 rounded-lg font-medium hover:bg-blue-700 transition">
                            Search Jobs <i class="fas fa-search ml-2"></i>
                        </button>
                    </div>
                </div>
            </div>
            
            <!-- Job Listings -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Job Card 1 -->
                <div class="job-card bg-white border rounded-lg overflow-hidden shadow-md transition duration-300 ease-in-out">
                    <div class="p-6">
                        <div class="flex justify-between items-start mb-4">
                            <div>
                                <h3 class="text-xl font-bold">Senior Software Engineer</h3>
                                <p class="text-gray-600">TechSolutions Inc.</p>
                            </div>
                            <div class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm font-medium">
                                Remote
                            </div>
                        </div>
                        <div class="flex items-center text-gray-600 mb-4">
                            <i class="fas fa-map-marker-alt mr-2"></i>
                            <span>San Francisco, CA (Remote)</span>
                        </div>
                        <div class="flex items-center text-gray-600 mb-4">
                            <i class="fas fa-dollar-sign mr-2"></i>
                            <span>$120,000 - $150,000/year</span>
                        </div>
                        <p class="text-gray-700 mb-4">We're looking for an experienced software engineer to join our team and help build the next generation of our platform.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-gray-500">Posted 2 days ago</span>
                            <button class="bg-blue-600 text-white px-4 py-2 rounded-lg text-sm font-medium hover:bg-blue-700 transition">
                                Apply Now
                            </button>
                        </div>
                    </div>
                </div>
                
                <!-- Job Card 2 -->
                <div class="job-card bg-white border rounded-lg overflow-hidden shadow-md transition duration-300 ease-in-out">
                    <div class="p-6">
                        <div class="flex justify-between items-start mb-4">
                            <div>
                                <h3 class="text-xl font-bold">Marketing Manager</h3>
                                <p class="text-gray-600">Growth Marketing Co.</p>
                            </div>
                            <div class="bg-green-100 text-green-800 px-3 py-1 rounded-full text-sm font-medium">
                                Full-time
                            </div>
                        </div>
                        <div class="flex items-center text-gray-600 mb-4">
                            <i class="fas fa-map-marker-alt mr-2"></i>
                            <span>New York, NY</span>
                        </div>
                        <div class="flex items-center text-gray-600 mb-4">
                            <i class="fas fa-dollar-sign mr-2"></i>
                            <span>$90,000 - $110,000/year</span>
                        </div>
                        <p class="text-gray-700 mb-4">Lead our marketing team to develop and execute strategies that drive customer acquisition and brand awareness.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-gray-500">Posted 1 week ago</span>
                            <button class="bg-blue-600 text-white px-4 py-2 rounded-lg text-sm font-medium hover:bg-blue-700 transition">
                                Apply Now
                            </button>
                        </div>
                    </div>
                </div>
                
                <!-- Job Card 3 -->
                <div class="job-card bg-white border rounded-lg overflow-hidden shadow-md transition duration-300 ease-in-out">
                    <div class="p-6">
                        <div class="flex justify-between items-start mb-4">
                            <div>
                                <h3 class="text-xl font-bold">UX/UI Designer</h3>
                                <p class="text-gray-600">Creative Design Studio</p>
                            </div>
                            <div class="bg-purple-100 text-purple-800 px-3 py-1 rounded-full text-sm font-medium">
                                Contract
                            </div>
                        </div>
                        <div class="flex items-center text-gray-600 mb-4">
                            <i class="fas fa-map-marker-alt mr-2"></i>
                            <span>Chicago, IL (Hybrid)</span>
                        </div>
                        <div class="flex items-center text-gray-600 mb-4">
                            <i class="fas fa-dollar-sign mr-2"></i>
                            <span>$50 - $70/hour</span>
                        </div>
                        <p class="text-gray-700 mb-4">Join our design team to create beautiful, intuitive interfaces for our clients across various industries.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-gray-500">Posted 3 days ago</span>
                            <button class="bg-blue-600 text-white px-4 py-2 rounded-lg text-sm font-medium hover:bg-blue-700 transition">
                                Apply Now
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-8">
                <button class="bg-white border border-blue-600 text-blue-600 px-6 py-3 rounded-lg font-medium hover:bg-blue-50 transition">
                    View All Jobs <i class="fas fa-arrow-right ml-2"></i>
                </button>
            </div>
        </div>
    </section>

    <!-- For Employers Section -->
    <section id="employers" class="py-16 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Hire Smarter With JobConnect Pro</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-12">
                <!-- Feature 1 -->
                <div class="bg-white p-6 rounded-lg shadow-md text-center">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-bolt text-4xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Automated Job Imports</h3>
                    <p class="text-gray-700">Automatically import jobs from Indeed, ZipRecruiter, and other platforms to expand your candidate pool.</p>
                </div>
                
                <!-- Feature 2 -->
                <div class="bg-white p-6 rounded-lg shadow-md text-center">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-video text-4xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Video Interviews</h3>
                    <p class="text-gray-700">Conduct live or pre-recorded video interviews directly in our platform with built-in evaluation tools.</p>
                </div>
                
                <!-- Feature 3 -->
                <div class="bg-white p-6 rounded-lg shadow-md text-center">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-chart-line text-4xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Advanced Analytics</h3>
                    <p class="text-gray-700">Track candidate progress, source effectiveness, and hiring metrics with our comprehensive dashboard.</p>
                </div>
            </div>
            
            <div class="bg-white rounded-lg shadow-xl overflow-hidden">
                <div class="md:flex">
                    <div class="md:w-1/2 p-8 md:p-12">
                        <h3 class="text-2xl font-bold mb-4">Complete Hiring Solution</h3>
                        <p class="text-gray-700 mb-6">From sourcing to screening to hiring, our platform provides all the tools you need to find and hire top talent efficiently.</p>
                        
                        <div class="space-y-4">
                            <div class="flex items-start">
                                <div class="text-green-500 mt-1 mr-3">
                                    <i class="fas fa-check-circle"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold">Applicant Tracking System</h4>
                                    <p class="text-gray-600 text-sm">Organize and manage candidates through every stage of your hiring process.</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="text-green-500 mt-1 mr-3">
                                    <i class="fas fa-check-circle"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold">Automated Screening</h4>
                                    <p class="text-gray-600 text-sm">Custom questionnaires and skill assessments to filter candidates.</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="text-green-500 mt-1 mr-3">
                                    <i class="fas fa-check-circle"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold">Collaborative Hiring</h4>
                                    <p class="text-gray-600 text-sm">Share feedback and notes with your team to make better hiring decisions.</p>
                                </div>
                            </div>
                        </div>
                        
                        <button class="mt-8 bg-blue-600 text-white px-6 py-3 rounded-lg font-medium hover:bg-blue-700 transition">
                            Get Started <i class="fas fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                    <div class="md:w-1/2 bg-gray-50 flex items-center justify-center p-8">
                        <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1350&q=80" alt="Hiring Dashboard" class="rounded-lg shadow-md">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section id="pricing" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-4">Simple, Transparent Pricing</h2>
            <p class="text-xl text-gray-600 text-center mb-12">Choose the plan that fits your hiring needs</p>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-5xl mx-auto">
                <!-- Basic Plan -->
                <div class="border rounded-lg shadow-sm hover:shadow-md transition">
                    <div class="p-6 border-b">
                        <h3 class="text-xl font-bold mb-2">Basic</h3>
                        <p class="text-gray-600 mb-4">For small businesses with occasional hiring needs</p>
                        <div class="mb-4">
                            <span class="text-4xl font-bold">$99</span>
                            <span class="text-gray-600">/month</span>
                        </div>
                        <button class="w-full bg-gray-200 text-gray-800 px-4 py-2 rounded-lg font-medium hover:bg-gray-300 transition">
                            Get Started
                        </button>
                    </div>
                    <div class="p-6">
                        <ul class="space-y-3">
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>1 Job Posting</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>50 Candidate Applications</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>Basic Screening Questions</span>
                            </li>
                            <li class="flex items-center text-gray-400">
                                <i class="fas fa-times text-red-400 mr-2"></i>
                                <span>No Video Interviews</span>
                            </li>
                            <li class="flex items-center text-gray-400">
                                <i class="fas fa-times text-red-400 mr-2"></i>
                                <span>No Automated Job Imports</span>
                            </li>
                        </ul>
                    </div>
                </div>
                
                <!-- Professional Plan (Featured) -->
                <div class="border-2 border-blue-500 rounded-lg shadow-md transform scale-105 z-10">
                    <div class="bg-blue-500 text-white text-center py-2 rounded-t-lg">
                        <span class="font-bold">MOST POPULAR</span>
                    </div>
                    <div class="p-6 border-b">
                        <h3 class="text-xl font-bold mb-2">Professional</h3>
                        <p class="text-gray-600 mb-4">For growing businesses with regular hiring</p>
                        <div class="mb-4">
                            <span class="text-4xl font-bold">$299</span>
                            <span class="text-gray-600">/month</span>
                        </div>
                        <button class="w-full bg-blue-600 text-white px-4 py-2 rounded-lg font-medium hover:bg-blue-700 transition">
                            Get Started
                        </button>
                    </div>
                    <div class="p-6">
                        <ul class="space-y-3">
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>5 Job Postings</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>Unlimited Applications</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>Advanced Screening</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>5 Video Interviews</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>Automated Job Imports</span>
                            </li>
                        </ul>
                    </div>
                </div>
                
                <!-- Enterprise Plan -->
                <div class="border rounded-lg shadow-sm hover:shadow-md transition">
                    <div class="p-6 border-b">
                        <h3 class="text-xl font-bold mb-2">Enterprise</h3>
                        <p class="text-gray-600 mb-4">For large organizations with high-volume hiring</p>
                        <div class="mb-4">
                            <span class="text-4xl font-bold">$599</span>
                            <span class="text-gray-600">/month</span>
                        </div>
                        <button class="w-full bg-gray-200 text-gray-800 px-4 py-2 rounded-lg font-medium hover:bg-gray-300 transition">
                            Get Started
                        </button>
                    </div>
                    <div class="p-6">
                        <ul class="space-y-3">
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>Unlimited Job Postings</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>Unlimited Applications</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>Custom Screening</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>Unlimited Video Interviews</span>
                            </li>
                            <li class="flex items-center">
                                <i class="fas fa-check text-green-500 mr-2"></i>
                                <span>Premium Job Imports</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            
            <div class="mt-12 bg-gray-100 p-8 rounded-lg max-w-4xl mx-auto">
                <h3 class="text-2xl font-bold mb-4 text-center">Pay-Per-Posting Option</h3>
                <div class="flex flex-col md:flex-row items-center justify-between">
                    <div class="mb-4 md:mb-0">
                        <p class="text-gray-700">Need to post just one job? Try our pay-per-posting option.</p>
                    </div>
                    <div class="flex items-center">
                        <span class="text-3xl font-bold mr-2">$300</span>
                        <span class="text-gray-600">per job posting</span>
                        <button class="ml-6 bg-blue-600 text-white px-6 py-2 rounded-lg font-medium hover:bg-blue-700 transition">
                            Post a Job
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="py-16 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">What Our Customers Say</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                        <span class="text-gray-600">2 weeks ago</span>
                    </div>
                    <p class="text-gray-700 mb-4">"JobConnect Pro has transformed our hiring process. The automated job imports save us hours of work each week, and the video interview feature is incredibly convenient."</p>
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/women/43.jpg" alt="Sarah Johnson" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold">Sarah Johnson</h4>
                            <p class="text-gray-600 text-sm">HR Director, TechStart Inc.</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                        <span class="text-gray-600">1 month ago</span>
                    </div>
                    <p class="text-gray-700 mb-4">"As a small business owner, I needed an affordable but powerful hiring solution. JobConnect Pro gave me access to features I thought were only for big companies."</p>
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Michael Chen" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold">Michael Chen</h4>
                            <p class="text-gray-600 text-sm">Founder, GreenLeaf Marketing</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star-half-alt"></i>
                        </div>
                        <span class="text-gray-600">3 days ago</span>
                    </div>
                    <p class="text-gray-700 mb-4">"The candidate tracking and analytics have helped us improve our hiring metrics significantly. We've reduced time-to-hire by 40% since switching to JobConnect Pro."</p>
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/women/65.jpg" alt="Emily Rodriguez" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold">Emily Rodriguez</h4>
                            <p class="text-gray-600 text-sm">Talent Acquisition, Global Corp</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Video Interview Demo -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-10 md:mb-0 md:pr-10">
                    <h2 class="text-3xl font-bold mb-6">Revolutionize Your Interviews</h2>
                    <p class="text-gray-700 mb-6">Our built-in video interview platform allows you to conduct live or pre-recorded interviews with candidates from anywhere in the world.</p>
                    
                    <div class="space-y-4">
                        <div class="flex items-start">
                            <div class="text-blue-500 mt-1 mr-3">
                                <i class="fas fa-check-circle"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Live Video Calls</h4>
                                <p class="text-gray-600">Conduct face-to-face interviews with our high-quality video platform.</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="text-blue-500 mt-1 mr-3">
                                <i class="fas fa-check-circle"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Pre-recorded Questions</h4>
                                <p class="text-gray-600">Send candidates questions to answer on their own time.</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="text-blue-500 mt-1 mr-3">
                                <i class="fas fa-check-circle"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Collaborative Evaluation</h4>
                                <p class="text-gray-600">Team members can review and rate candidate responses.</p>
                            </div>
                        </div>
                    </div>
                    
                    <button class="mt-8 bg-blue-600 text-white px-6 py-3 rounded-lg font-medium hover:bg-blue-700 transition">
                        Try Video Interviews
                    </button>
                </div>
                <div class="md:w-1/2">
                    <div class="video-container rounded-lg shadow-xl overflow-hidden">
                        <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?autoplay=0&mute=1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Bank Integration Section -->
    <section class="py-16 bg-gray-100">
        <div class="container mx-auto px-4">
            <div class="bg-white rounded-lg shadow-xl overflow-hidden">
                <div class="md:flex">
                    <div class="md:w-1/2 p-8 md:p-12">
                        <h2 class="text-3xl font-bold mb-6">Easy Payment Setup</h2>
                        <p class="text-gray-700 mb-6">Connect your bank account in minutes to start receiving payments for your job postings and services.</p>
                        
                        <div class="space-y-4 mb-8">
                            <div class="flex items-center">
                                <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                    <i class="fas fa-university"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold">Secure Bank Connection</h4>
                                    <p class="text-gray-600">256-bit encryption keeps your financial information safe.</p>
                                </div>
                            </div>
                            
                            <div class="flex items-center">
                                <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                    <i class="fas fa-clock"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold">Fast Transfers</h4>
                                    <p class="text-gray-600">Payments deposited within 1-2 business days.</p>
                                </div>
                            </div>
                            
                            <div class="flex items-center">
                                <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                    <i class="fas fa-globe"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold">Global Support</h4>
                                    <p class="text-gray-600">Works with banks in over 50 countries.</p>
                                </div>
                            </div>
                        </div>
                        
                        <button id="connect-bank-btn" class="bg-blue-600 text-white px-6 py-3 rounded-lg font-medium hover:bg-blue-700 transition">
                            Connect Your Bank Account
                        </button>
                    </div>
                    <div class="md:w-1/2 bg-blue-50 flex items-center justify-center p-8">
                        <img src="https://images.unsplash.com/photo-1553729459-efe14ef6055d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1350&q=80" alt="Bank Integration" class="rounded-lg max-w-md w-full">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Social Proof Section -->
    <section class="py-12 bg-white">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-center items-center space-y-6 md:space-y-0 md:space-x-12">
                <div class="text-center">
                    <div class="text-4xl font-bold text-blue-600">10,000+</div>
                    <div class="text-gray-600">Companies Hiring</div>
                </div>
                <div class="text-center">
                    <div class="text-4xl font-bold text-blue-600">500,000+</div>
                    <div class="text-gray-600">Jobs Posted</div>
                </div>
                <div class="text-center">
                    <div class="text-4xl font-bold text-blue-600">5M+</div>
                    <div class="text-gray-600">Candidates Hired</div>
                </div>
                <div class="text-center">
                    <div class="text-4xl font-bold text-blue-600">98%</div>
                    <div class="text-gray-600">Customer Satisfaction</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Social Media Promotion -->
    <section class="py-16 bg-blue-600 text-white">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl font-bold mb-6">Join Our Growing Community</h2>
            <p class="text-xl mb-8 max-w-2xl mx-auto">Follow us on social media for hiring tips, success stories, and platform updates.</p>
            
            <div class="flex justify-center space-x-6 mb-12">
                <a href="#" class="bg-white text-blue-600 p-3 rounded-full w-12 h-12 flex items-center justify-center hover:bg-blue-100 transition">
                    <i class="fab fa-facebook-f"></i>
                </a>
                <a href="#" class="bg-white text-blue-600 p-3 rounded-full w-12 h-12 flex items-center justify-center hover:bg-blue-100 transition">
                    <i class="fab fa-twitter"></i>
                </a>
                <a href="#" class="bg-white text-blue-600 p-3 rounded-full w-12 h-12 flex items-center justify-center hover:bg-blue-100 transition">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="#" class="bg-white text-blue-600 p-3 rounded-full w-12 h-12 flex items-center justify-center hover:bg-blue-100 transition">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="#" class="bg-white text-blue-600 p-3 rounded-full w-12 h-12 flex items-center justify-center hover:bg-blue-100 transition">
                    <i class="fab fa-youtube"></i>
                </a>
            </div>
            
            <div class="bg-white text-gray-800 rounded-lg p-6 max-w-3xl mx-auto">
                <h3 class="text-2xl font-bold mb-4">Share Your Success Story</h3>
                <p class="mb-6">Have you had success using JobConnect Pro? We'd love to feature your story on our social channels!</p>
                <button class="bg-blue-600 text-white px-6 py-3 rounded-lg font-medium hover:bg-blue-700 transition">
                    Share Your Story
                </button>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Get In Touch</h2>
            
            <div class="flex flex-col md:flex-row">
                <div class="md:w-1/2 mb-10 md:mb-0 md:pr-10">
                    <h3 class="text-2xl font-bold mb-4">Contact Information</h3>
                    <p class="text-gray-700 mb-6">Have questions about our platform or need support? Reach out to our team.</p>
                    
                    <div class="space-y-4">
                        <div class="flex items-start">
                            <div class="text-blue-600 mt-1 mr-4">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Email</h4>
                                <p class="text-gray-600">support@jobconnectpro.com</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="text-blue-600 mt-1 mr-4">
                                <i class="fas fa-phone-alt"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Phone</h4>
                                <p class="text-gray-600">+1 (555) 123-4567</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="text-blue-600 mt-1 mr-4">
                                <i class="fas fa-map-marker-alt"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Office</h4>
                                <p class="text-gray-600">123 Hiring Street, Suite 500<br>San Francisco, CA 94107</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mt-8">
                        <h4 class="font-bold mb-2">Support Hours</h4>
                        <p class="text-gray-600">Monday - Friday: 8am - 8pm EST<br>Saturday: 9am - 5pm EST</p>
                    </div>
                </div>
                
                <div class="md:w-1/2 bg-gray-100 p-8 rounded-lg">
                    <h3 class="text-2xl font-bold mb-4">Send Us a Message</h3>
                    <form>
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">Name</label>
                            <input type="text" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                        </div>
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">Email</label>
                            <input type="email" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                        </div>
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">Subject</label>
                            <select class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                                <option>General Inquiry</option>
                                <option>Technical Support</option>
                                <option>Billing Question</option>
                                <option>Feature Request</option>
                            </select>
                        </div>
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">Message</label>
                            <textarea rows="4" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"></textarea>
                        </div>
                        <button type="submit" class="w-full bg-blue-600 text-white px-6 py-3 rounded-lg font-medium hover:bg-blue-700 transition">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Login Modal -->
    <div id="login-modal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 hidden">
        <div class="bg-white rounded-lg shadow-xl w-full max-w-md">
            <div class="p-6">
                <div class="flex justify-between items-center mb-6">
                    <h3 class="text-2xl font-bold">Login to Your Account</h3>
                    <button id="close-login-modal" class="text-gray-500 hover:text-gray-700">
                        <i class="fas fa-times"></i>
                    </button>
                </div>
                
                <form id="login-form">
                    <div class="mb-4">
                        <label class="block text-gray-700 mb-2">Email</label>
                        <input type="email" id="login-email" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" value="diallo2555@gmail.com">
                    </div>
                    <div class="mb-6">
                        <label class="block text-gray-700 mb-2">Password</label>
                        <input type="password" id="login-password" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" value="Montana22@">
                    </div>
                    <div class="flex items-center justify-between mb-4">
                        <div class="flex items-center">
                            <input type="checkbox" id="remember-me" class="mr-2">
                            <label for="remember-me" class="text-gray-700">Remember me</label>
                        </div>
                        <a href="#" class="text-blue-600 hover:underline">Forgot password?</a>
                    </div>
                    <button type="submit" class="w-full bg-blue-600 text-white px-6 py-3 rounded-lg font-medium hover:bg-blue-700 transition mb-4">
                        Login
                    </button>
                    <div class="text-center">
                        <span class="text-gray-600">Don't have an account?</span>
                        <a href="#" class="text-blue-600 hover:underline ml-2">Sign up</a>
                    </div>
                </form>
            </div>
        </div>
    </div>

    <!-- Bank Connection Modal -->
    <div id="bank-modal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 hidden">
        <div class="bg-white rounded-lg shadow-xl w-full max-w-2xl">
            <div class="p-6">
                <div class="flex justify-between items-center mb-6">
                    <h3 class="text-2xl font-bold">Connect Your Bank Account</h3>
                    <button id="close-bank-modal" class="text-gray-500 hover:text-gray-700">
                        <i class="fas fa-times"></i>
                    </button>
                </div>
                
                <div class="mb-8">
                    <div class="flex items-center mb-4">
                        <div class="w-8 h-8 bg-blue-600 text-white rounded-full flex items-center justify-center mr-3">1</div>
                        <h4 class="font-bold">Select Your Bank</h4>
                    </div>
                    <div class="ml-11 mb-6">
                        <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                            <button class="bank-logo p-4 border rounded-lg hover:bg-gray-50">
                                <img src="https://logo.clearbit.com/chase.com" alt="Chase" class="h-8 mx-auto">
                            </button>
                            <button class="bank-logo p-4 border rounded-lg hover:bg-gray-50">
                                <img src="https://logo.clearbit.com/bankofamerica.com" alt="Bank of America" class="h-8 mx-auto">
                            </button>
                            <button class="bank-logo p-4 border rounded-lg hover:bg-gray-50">
                                <img src="https://logo.clearbit.com/wellsfargo.com" alt="Wells Fargo" class="h-8 mx-auto">
                            </button>
                            <button class="bank-logo p-4 border rounded-lg hover:bg-gray-50">
                                <img src="https://logo.clearbit.com/citi.com" alt="Citi" class="h-8 mx-auto">
                            </button>
                        </div>
                        <div class="mt-4">
                            <p class="text-gray-600">Can't find your bank? <a href="#" class="text-blue-600 hover:underline">Search for it</a></p>
                        </div>
                    </div>
                    
                    <div class="flex items-center mb-4">
                        <div class="w-8 h-8 bg-gray-300 text-white rounded-full flex items-center justify-center mr-3">2</div>
                        <h4 class="font-bold text-gray-400">Enter Your Credentials</h4>
                    </div>
                    
                    <div class="flex items-center mb-4">
                        <div class="w-8 h-8 bg-gray-300 text-white rounded-full flex items-center justify-center mr-3">3</div>
                        <h4 class="font-bold text-gray-400">Verify Your Account</h4>
                    </div>
                </div>
                
                <div class="bg-gray-100 p-4 rounded-lg">
                    <div class="flex items-start">
                        <div class="text-blue-500 mt-1 mr-3">
                            <i class="fas fa-lock"></i>
                        </div>
                        <div>
                            <h4 class="font-bold mb-1">Security Information</h4>
                            <p class="text-gray-600 text-sm">We use bank-level 256-bit encryption to protect your information. Your banking credentials are never stored on our servers.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Login Success Toast -->
    <div id="login-toast" class="fixed bottom-4 right-4 bg-green-500 text-white px-6 py-3 rounded-lg shadow-lg flex items-center hidden z-50">
        <i class="fas fa-check-circle mr-3"></i>
        <span>Successfully logged in as diallo2555@gmail.com</span>
        <button id="close-toast" class="ml-4">
            <i class="fas fa-times"></i>
        </button>
    </div>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-8">
                <div>
                    <h4 class="text-xl font-bold mb-4 flex items-center">
                        <i class="fas fa-handshake mr-2"></i>
                        <span>JobConnect Pro</span>
                    </h4>
                    <p class="text-gray-400">The most comprehensive hiring platform connecting top talent with great companies worldwide.</p>
                </div>
                <div>
                    <h4 class="text-lg font-bold mb-4">For Candidates</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Browse Jobs</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Create Profile</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Job Alerts</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Career Resources</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-bold mb-4">For Employers</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Post a Job</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Browse Candidates</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Pricing Plans</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Hiring Resources</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-bold mb-4">Company</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">About Us</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Careers</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Contact</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Blog</a></li>
                    </ul>
                </div>
            </div>
            <div class="pt-8 border-t border-gray-800">
                <div class="flex flex-col md:flex-row justify-between items-center">
                    <p class="text-gray-400 mb-4 md:mb-0">© 2023 JobConnect Pro. All rights reserved.</p>
                    <div class="flex space-x-6">
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-instagram"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const closeSidebarButton = document.getElementById('close-sidebar');
        const sidebar = document.getElementById('sidebar');
        
        mobileMenuButton.addEventListener('click', () => {
            sidebar.classList.add('open');
        });
        
        closeSidebarButton.addEventListener('click', () => {
            sidebar.classList.remove('open');
        });
        
        // Login Modal
        const loginButton = document.getElementById('login-btn');
        const loginModal = document.getElementById('login-modal');
        const closeLoginModal = document.getElementById('close-login-modal');
        const loginForm = document.getElementById('login-form');
        const loginToast = document.getElementById('login-toast');
        const closeToast = document.getElementById('close-toast');
        
        loginButton.addEventListener('click', () => {
            loginModal.classList.remove('hidden');
        });
        
        closeLoginModal.addEventListener('click', () => {
            loginModal.classList.add('hidden');
        });
        
        loginForm.addEventListener('submit', (e) => {
            e.preventDefault();
            const email = document.getElementById('login-email').value;
            const password = document.getElementById('login-password').value;
            
            // Simple validation
            if (email === 'diallo2555@gmail.com' && password === 'Montana22@') {
                loginModal.classList.add('hidden');
                loginToast.classList.remove('hidden');
                
                // Hide toast after 5 seconds
                setTimeout(() => {
                    loginToast.classList.add('hidden');
                }, 5000);
            } else {
                alert('Invalid email or password. For this demo, use:\nEmail: diallo2555@gmail.com\nPassword: Montana22@');
            }
        });
        
        closeToast.addEventListener('click', () => {
            loginToast.classList.add('hidden');
        });
        
        // Bank Connection Modal
        const bankButton = document.getElementById('connect-bank-btn');
        const bankModal = document.getElementById('bank-modal');
        const closeBankModal = document.getElementById('close-bank-modal');
        
        bankButton.addEventListener('click', () => {
            bankModal.classList.remove('hidden');
        });
        
        closeBankModal.addEventListener('click', () => {
            bankModal.classList.add('hidden');
        });
        
        // Bank logo selection
        const bankLogos = document.querySelectorAll('.bank-logo');
        bankLogos.forEach(logo => {
            logo.addEventListener('click', () => {
                // Remove active class from all logos
                bankLogos.forEach(l => {
                    l.classList.remove('border-blue-500', 'bg-blue-50');
                });
                // Add active class to clicked logo
                logo.classList.add('border-blue-500', 'bg-blue-50');
            });
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    sidebar.classList.remove('open');
                }
            });
        });
    </script>
</body>
</html>
