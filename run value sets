<%@ page import="webemr.analytics.cmsdata.service.ExcelToTableService" %>
<%@ page import="com.ecw.filetransfer.utility.PathFactory" %>
<%@ page import="java.io.File" %>
<%@ page import="java.util.Map" %>
<%
    ExcelToTableService excelToTableService = new ExcelToTableService();
    String directoryPath= PathFactory.WEBAPPS_PATH.getPath()+ File.separatorChar+"mobiledoc"+File.separatorChar+"jsp"+File.separatorChar+"webemr"+File.separatorChar+"analytics"+File.separatorChar+"cmsdata"+File.separatorChar+"excel"+File.separatorChar;
    Map<String,String> result= excelToTableService.parseFile(directoryPath);
    if(result!=null){
      out.print(result.get("msg"));
    }
%>
