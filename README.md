import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { FaLinkedin, FaEnvelope, FaFileDownload } from "react-icons/fa";
import Image from "next/image";

const Portfolio = () => {
  return (
    <div className="min-h-screen bg-gradient-to-r from-blue-100 to-purple-200 flex flex-col items-center p-8">
      <Card className="w-full max-w-4xl bg-white shadow-2xl rounded-2xl p-6 border border-gray-300">
        <div className="flex flex-col items-center text-center">
          <Image
            src="https://drive.google.com/file/d/1KtkJCGqqJn9YU_pPvKCeaLJSrB2l4Uvu/view?usp=sharing"
            alt="Jayasree M"
            width={150}
            height={150}
            className="rounded-full border-4 border-blue-500 shadow-md"
            priority={true}
          />
          <h1 className="text-4xl font-extrabold text-gray-800 mt-4">Jayasree M</h1>
          <p className="text-gray-600 text-lg italic">Data Analyst | Excel | Power BI | SQL</p>
        </div>
        
        <CardContent className="mt-6 space-y-6 text-gray-700">
          <section>
            <h2 className="text-2xl font-semibold text-blue-600">About Me</h2>
            <p>
              I'm a passionate Data Analyst with expertise in data cleaning, visualization, 
              and dashboard creation. I enjoy transforming raw data into meaningful insights.
            </p>
          </section>

          <section>
            <h2 className="text-2xl font-semibold text-blue-600">Skills</h2>
            <ul className="list-disc pl-6 space-y-2">
              <li>Data Cleaning (Text Formatting, Removing Duplicates, Power Query)</li>
              <li>Data Visualization (Charts, Color Formatting, Dashboards)</li>
              <li>Pivot Table Analysis (Filters, Calculated Values, Percentage Analysis)</li>
              <li>Dashboard Creation (Meaningful Chart Arrangements)</li>
              <li>SQL (Queries, Data Manipulation, Joins)</li>
            </ul>
          </section>

          <section>
            <h2 className="text-2xl font-semibold text-blue-600">Featured Project</h2>
            <p>
              <strong>Gen Z Career Aspirations Analysis</strong> – Worked with a dataset of 4000+ entries,
              performing data cleaning, visualization, pivot analysis, and dashboard creation
              using Excel and Power BI.
            </p>
          </section>

          <section>
            <h2 className="text-2xl font-semibold text-blue-600">Internships</h2>
            <ul className="list-disc pl-6 space-y-2">
              <li>Data Analytics Intern – KultureHire</li>
              <li>Data Visualization Intern – Cognifyz Technologies</li>
            </ul>
          </section>

          <section>
            <h2 className="text-2xl font-semibold text-blue-600">Certifications</h2>
            <ul className="list-disc pl-6 space-y-2">
              <li>Excel: Mother of Business Intelligence – Codebasics</li>
              <li>Data Cleaning Frameworks and Techniques – Data Professionals</li>
              <li>Microsoft Excel: Pivot Tables Analysis Beginner to Pro</li>
              <li>Excel Dashboarding</li>
              <li>Data Storytelling for Data Professionals</li>
              <li>Problem Solving and Documenting Problem Statements + ChatGPT</li>
            </ul>
          </section>
        </CardContent>
        
        <div className="flex justify-center space-x-4 mt-6">
          <Button asChild className="bg-blue-500 hover:bg-blue-600 text-white px-4 py-2 rounded-lg shadow-md">
            <a href="https://www.linkedin.com/in/jayasree-m-428ba42a6/" target="_blank" rel="noopener noreferrer">
              <FaLinkedin className="mr-2" /> LinkedIn
            </a>
          </Button>
          <Button asChild className="bg-green-500 hover:bg-green-600 text-white px-4 py-2 rounded-lg shadow-md">
            <a href="mailto:jayasree.m1043@gmail.com">
              <FaEnvelope className="mr-2" /> Email
            </a>
          </Button>
          <Button asChild className="bg-purple-500 hover:bg-purple-600 text-white px-4 py-2 rounded-lg shadow-md">
            <a href="https://drive.google.com/file/d/1LcfTU6e_vPe_mRBs3cchAfVK1OItMnAT/view?usp=sharing" download>
              <FaFileDownload className="mr-2" /> Download CV
            </a>
          </Button>
        </div>
      </Card>
    </div>
  );
};

export default Portfolio;
