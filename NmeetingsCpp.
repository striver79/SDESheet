int maxMeetings(int start[], int end[], int n)
    {
        
        vector<pair<int,int>> intervals;
        for(int i=0; i<n; i++)
        {
            intervals.push_back({start[i],end[i]});
        }
        sort(intervals.begin(),intervals.end());
        int sol=1, endTime=intervals[0].second;
        for(int i=1; i<n; i++)
        {
            if(endTime<intervals[i].first)
            {
                sol++;
                endTime=intervals[i].second;
            }
            else
                endTime=min(endTime,intervals[i].second);
        }
        return sol;
    }
